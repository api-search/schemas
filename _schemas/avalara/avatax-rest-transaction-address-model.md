---
description: TransactionAddressModel schema from Avalara API
layout: schema
name: TransactionAddressModel
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: line1
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: region
  type: string
- description: ''
  name: postalCode
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: latitude
  type: number
- description: ''
  name: longitude
  type: number
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-transaction-address-model-schema.json
slug: avatax-rest-transaction-address-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-transaction-address-model-schema.json\",\n  \"title\": \"TransactionAddressModel\",\n  \"description\": \"TransactionAddressModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"line1\": {\n      \"type\": \"string\"\n    },\n    \"city\": {\n      \"type\": \"string\"\n    },\n    \"region\": {\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"type\": \"string\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-transaction-address-model-schema.json
tags:
- Taxes
title: TransactionAddressModel
---
