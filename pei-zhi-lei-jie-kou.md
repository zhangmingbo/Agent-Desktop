| URL | [/v1/platform/config/agent/add\_agent](http://localhost:8090/swagger-ui.html#!/AgentInfoController/addAgentInfoUsingPOST) |
| :--- | :--- |
| HTTP Method | POST |
| 功能描述 | 创建一个新员工，并同步到语音平台 |
| 输入 | 报文JSON：{"active": 0,"agentId": "","agentName": "","canRoute": true,"captainLevel": 0,"channelType": "","password": "","role": "string","serviceAbility": 0,"skillId": “","agentGroupId": “","businessGroupId": "","tenantId": "","userId": ""} |
| 输出 | {"retCode":1, //返回码，具体见附录A"msg": "", //返回消息内容} |
| 备注 | 如果skillId为空，不进行添加到座席组和技能的操作，如果skillId不为空，座席组Id或技能Id为空，则添加到默认的座席组或添加默认技能 |
|  | 示例：http://{ip}:{port}/v1/platform/config/agent/add\_agent |



