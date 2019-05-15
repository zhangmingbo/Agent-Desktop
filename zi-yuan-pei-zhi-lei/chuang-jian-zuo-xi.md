---
description: 创建一个新员工
---

# 创建座席

{% api-method method="post" host="https://api.cakes.com" path="/v1/platform/config/agent/add\_agent" %}
{% api-method-summary %}
新建座席账号
{% endapi-method-summary %}

{% api-method-description %}
创建座席，并赋予属性
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Authentication" type="string" required=true %}
Authentication token to track down who is emptying our stocks.
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="userId" type="string" required=false %}
用户登陆ID
{% endapi-method-parameter %}

{% api-method-parameter name="serviceAbility" type="integer" required=false %}
并发处理能力
{% endapi-method-parameter %}

{% api-method-parameter name="channelType" type="string" required=true %}
渠道列表\(webchat,wechat,call,appchat\)
{% endapi-method-parameter %}

{% api-method-parameter name="captainLevel" type="string" required=true %}
班长等级
{% endapi-method-parameter %}

{% api-method-parameter name="canRoute" type="boolean" required=true %}
是否可路由
{% endapi-method-parameter %}

{% api-method-parameter name="agentName" type="string" required=false %}
座席名称
{% endapi-method-parameter %}

{% api-method-parameter name="agentId" type="string" required=true %}
座席工号
{% endapi-method-parameter %}

{% api-method-parameter name="tenantId" type="string" required=true %}
租户ID
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{
  "retCode":1,   //返回码，具体见附录A
  "msg": "",     //返回消息内容
}

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



