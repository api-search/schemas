---
description: LineItemModel schema from Avalara API
layout: schema
name: LineItemModel
properties_list:
- description: Line number within the transaction
  name: number
  type: string
- description: Quantity of items
  name: quantity
  type: number
- description: Total amount for this line
  name: amount
  type: number
- description: Tax code for this line item
  name: taxCode
  type: string
- description: Item code for the product or service
  name: itemCode
  type: string
- description: Description of the line item
  name: description
  type: string
- description: ''
  name: addresses
  type: object
- description: Exemption code for tax-exempt purchases
  name: exemptionCode
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-line-item-model-schema.json
slug: avatax-rest-line-item-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-line-item-model-schema.json\",\n  \"title\": \"LineItemModel\",\n  \"description\": \"LineItemModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"amount\"\n  ],\n  \"properties\": {\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Line number within the transaction\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"default\": 1,\n      \"description\": \"Quantity of items\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total amount for this line\"\n    },\n    \"taxCode\": {\n      \"type\": \"string\",\n      \"description\": \"Tax code for this line item\"\n    },\n    \"itemCode\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Item code for the product or service\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the line item\"\n    },\n    \"addresses\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"shipFrom\": {\n          \"$ref\": \"#/components/schemas/AddressInfo\"\n        },\n        \"shipTo\": {\n          \"$ref\": \"#/components/schemas/AddressInfo\"\n        }\n      }\n    },\n    \"exemptionCode\": {\n      \"type\": \"string\",\n      \"description\": \"Exemption code for tax-exempt purchases\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-line-item-model-schema.json
tags:
- Taxes
title: LineItemModel
---
