---
description: Database connection string value to type pair.
layout: schema
name: ConnStringValueTypePair
properties_list:
- description: Type of database.
  name: type
  type: string
- description: Value of pair.
  name: value
  type: string
provider_name: Azure Function Apps
provider_slug: azure-function-apps
schema_file: json-schema/azure-function-apps-conn-string-value-type-pair-schema.json
slug: azure-function-apps-conn-string-value-type-pair
source_filename: azure-function-apps-conn-string-value-type-pair-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-conn-string-value-type-pair-schema.json\",\n  \"title\": \"ConnStringValueTypePair\",\n  \"description\": \"Database connection string value to type pair.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"description\": \"Type of database.\",\n      \"enum\": [\n        \"MySql\",\n        \"SQLServer\",\n        \"SQLAzure\",\n        \"Custom\",\n        \"NotificationHub\",\n        \"ServiceBus\",\n        \"EventHub\",\n        \"ApiHub\",\n        \"DocDb\",\n        \"RedisCache\",\n        \"PostgreSQL\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"ConnectionStringType\"\n      }\n    },\n    \"value\": {\n      \"description\": \"Value of pair.\",\n      \"type\": \"string\"\
  \n    }\n  },\n  \"required\": [\n    \"value\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-conn-string-value-type-pair-schema.json
tags:
- Azure
- Compute
- FaaS
- Functions
- Serverless
title: ConnStringValueTypePair
---
