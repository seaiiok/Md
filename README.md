protoc-gen-tier - generate code.
===================
简介
-------------
使用protoc-gen-tier 生成代码,接口UI文档,Postman文档。

描述
-------------
1.apis 
使用：protoc-gen-postman-doc
(postman文档无manifest,因为它生成需要的数据包含在apis里面了)。 
增加option来增强对接口的说明，这对后面的接口文档和postman文档生成都有很大的帮助。

如下：
```proto
// 获取参与节点信息 (2.13)
rpc GetParticipantNodeInfoById(kuaicuocuo.com.apis.ssi.fe.v1.common.FENodeId) returns (FERespParticipantNodeInfo){
    //该方法全局唯一的名字，暂定: 服务名/方法名 (service name/method name)
    option (kuaicuocuo.com.api.doc).api_name = "FEGovernanFEGceOrgService/GetParticipantNodeInfoById"
    option (google.api.http) = {
            //url 在manifest里说明url前缀
            //post:""
            get:"/FEGovernanFEGceOrgService/GetParticipantNodeInfoById?node_id=?"
            //请求body
            body:'{"name":"body"}'
            //响应body
            response_body:'{"name":"response body"}'
    };
    //TODO 建议去除
    //option (kuaicuocuo.com.api.doc) = {
    //      //该接口的分类名，影响postman结构，可以不说明，因为postman结构和service是统一的
    //      category_name:"治理组织"
    //}
};
```

2.manifest--generate code
使用：protoc-gen-tier
服务代码的生成和Postman文档的生成。

如下：
```proto
option (kuaicuocuo.com.api.app).manifest = {
        modules:{key:"fe_operator",value:{
              //服务名 server name
              register_service_name:"fe-operator-service"
              //指定输出服务
              expose_service:"FEOperatorService"
              //指定依赖模块服务
              dependent_modules:["operator"]
        }}
}
```

3.manifest--generate doc
使用：protoc-gen-ui-doc
用于描述UI与接口业务关系的文档，明确指指定UI图片对应的接口列表。

如下：
```proto
option (kuaicuocuo.com.api.doc).doc = {
       uis:{key:"ui001",value:{
              name:"创建联盟"
              //ui图片相对路径
              path:"/01-添加治理联盟/01创建联盟.png",
              //接口唯一方法名字
              urls:["FEGovernanFEGceOrgService/GetParticipantNodeInfoById"]
        }}
}
```

//TODO 后期完善使用文档
//TODO 终端动画教程
Quick Start
-------------
* 1.首先修改sample文件后缀为go文件.
* 2.可选:在Init中初始化服务.
* 3.可选:在服务中添加逻辑.
* 4.cd kcc_micro_api, make run 启动micro.
* 5.本目录中 make run 启动微服务.