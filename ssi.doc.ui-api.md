---
typora-root-url: ./2020-02-05
---

## 环境变量

HostName: 192.168.1.6:8080

------


## ui001 - 创建联盟

![](./2020-02-05/dccae8f0cb1cfa5538729847ad9039ab.png)


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

![](2020-02-05/0ccd0adec635ff0560c5d199a1fdfc37.png)



## ui003 - 登录

![](./2020-02-05/bee42fa65571968ab1f4f457eb2648de.png)


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

![](./2020-02-05/57ea8946ae22a988f9d7f52251a9b87b.png)


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

![](./2020-02-05/7e980d772be45e8663de6c8b1d42e1a3.png)


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

![](./2020-02-05/f8417d779c6f5ad9e6e6bbe847db2f7c.png)



