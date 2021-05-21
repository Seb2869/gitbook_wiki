---
description: Community Java server
---

# Ethparser contracts API

{% api-method method="get" host="http://ethparser.herokuapp.com" path="/contracts/vaults" %}
{% api-method-summary %}
Vaults contracts
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="network" type="string" required=false %}
eth or bsc
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
	"code": "200",
	"status": "OK",
	"data": [
		{
			"id": 123,
			"contract": {
				"id": 516,
				"address": "0x274aa8b58e8c57c4e347c8768ed853eb6d375b48",
				"name": "SUSHI",
				"created": 11954197,
				"updated": 12134782,
				"type": 0,
				"network": "eth",
				"underlying": null
			},
			"updatedBlock": 11954197,
			"controller": {
				"id": 146,
				"address": "0x222412af183bceadefd72e4cb1b71f1889953b1c",
				"name": "CONTROLLER",
				"created": 0,
				"updated": null,
				"type": 3,
				"network": "eth",
				"underlying": null
			},
			"governance": {
				"id": 147,
				"address": "0xf00dd244228f51547f0563e60bca65a30fbf5f7f",
				"name": "GOVERNANCE",
				"created": 0,
				"updated": null,
				"type": 3,
				"network": "eth",
				"underlying": null
			},
			"strategy": null,
			"underlying": {
				"id": 171,
				"address": "0x6b3595068778dd592e39a122f4f5a5cf09c90fe2",
				"name": "SUSHI",
				"created": 10776509,
				"updated": 12134782,
				"type": 4,
				"network": "eth",
				"underlying": null
			},
			"name": "FARM_SUSHI",
			"symbol": "fSUSHI",
			"decimals": 18,
			"underlyingUnit": 1000000000000000000
		}
	]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="http://ethparser.herokuapp.com" path="/contracts/pools" %}
{% api-method-summary %}
Pools contracts
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="network" type="string" required=false %}
eth or bsc
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="http://ethparser.herokuapp.com" path="/contracts/tokens" %}
{% api-method-summary %}
Related Tokens Contracts
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="network" type="string" required=false %}
eth or bsc
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="http://ethparser.herokuapp.com" path="/contracts/lps" %}
{% api-method-summary %}
Related Liquidity Pools Contracts
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="network" type="string" required=false %}
eth or bsc
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

