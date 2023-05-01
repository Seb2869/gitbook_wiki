---
description: Community Java server
---

# Ethparser contracts API

{% swagger baseUrl="http://ethparser.herokuapp.com" path="/contracts/vaults" method="get" summary="Vaults contracts" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="network" type="string" %}
eth or bsc
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
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
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="http://ethparser.herokuapp.com" path="/contracts/pools" method="get" summary="Pools contracts" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="network" type="string" %}
eth or bsc
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="http://ethparser.herokuapp.com" path="/contracts/tokens" method="get" summary="Related Tokens Contracts" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="network" type="string" %}
eth or bsc
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="http://ethparser.herokuapp.com" path="/contracts/lps" method="get" summary="Related Liquidity Pools Contracts" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="network" type="string" %}
eth or bsc
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
```
{% endswagger-response %}
{% endswagger %}
