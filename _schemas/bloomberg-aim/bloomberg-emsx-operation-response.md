---
description: ''
layout: schema
name: OperationResponse
properties_list:
- description: Operation status code (0 = success)
  name: STATUS
  type: integer
- description: Status message
  name: MESSAGE
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-operation-response-schema.json
slug: bloomberg-emsx-operation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OperationResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"STATUS\": {\n      \"type\": \"integer\",\n      \"description\": \"Operation status code (0 = success)\"\n    },\n    \"MESSAGE\": {\n      \"type\": \"string\",\n      \"description\": \"Status message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-operation-response-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: OperationResponse
---
