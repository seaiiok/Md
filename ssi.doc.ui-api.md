---
typora-root-url: Git.2020-02-05
---

## 环境变量

HostName: 192.168.1.6:8080

------


## ui001 - 创建联盟

![](/0dc106fe111d2aaee0724db6ae66669b.png)


FEGovernancePanelService-CreateGovernancePanel
方法: POST
路径: http://{{HostName}}/fe-panel-service/FEGovernancePanelService/CreateGovernancePanel
请求示例(json): {
					"login_id":"xx",
					"login_password":"1234"
				}	
				
响应示例(json): {
				    	"code":100,
					"message":"success"
				}
				


FEGovernancePanelService-ListAllConsistencePolicys
方法: GET
路径: http://{{HostName}}/fe-panel-service/FEGovernancePanelService/ListAllConsistencePolicys
请求示例(json): {
					"login_id":"xx",
					"login_password":"1234"
				}	
				
响应示例(json): {
				    	"code":100,
					"message":"success"
				}
				



## ui002 - 创建成功

![](0dc106fe111d2aaee0724db6ae66669b.png)



## ui003 - 登录

![](0dc106fe111d2aaee0724db6ae66669b.png)


FEOperatorService-OperatorLogin
方法: POST
路径: http://{{HostName}}/fe-panel-service/FEOperatorService/OperatorLogin
请求示例(json): {
					"login_id":"xx",
					"login_password":"1234"
				}	
				
响应示例(json): {
				    	"code":100,
					"message":"success"
				}
				



## ui004 - 申请加入

![](647df4e415eed3384b26463ba5360fa3.png)


FEApplyService-ApplyJoinPanel
方法: POST
路径: http://{{HostName}}/fe-panel-service/FEApplyService/ApplyJoinPanel
请求示例(json): {
					"login_id":"xx",
					"login_password":"1234"
				}	
				
响应示例(json): {
				    	"code":100,
					"message":"success"
				}
				



## ui005 - 申请加入交互

![](8cc58026b935550b49736494ef9431b5.png)


FEGovernancePanelService-ListAllConsistencePolicys
方法: GET
路径: http://{{HostName}}/fe-panel-service/FEGovernancePanelService/ListAllConsistencePolicys
请求示例(json): {
					"login_id":"xx",
					"login_password":"1234"
				}	
				
响应示例(json): {
				    	"code":100,
					"message":"success"
				}
				



## ui006 - 申请成功

![](8b2e5417f17d65d353e095344dbc5e83.png)



