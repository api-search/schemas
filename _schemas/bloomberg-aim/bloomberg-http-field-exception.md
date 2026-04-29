---
description: ''
layout: schema
name: FieldException
properties_list:
- description: ''
  name: fieldId
  type: string
- description: ''
  name: errorInfo
  type: object
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-http-field-exception-schema.json
slug: bloomberg-http-field-exception
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FieldException\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldId\": {\n      \"type\": \"string\"\n    },\n    \"errorInfo\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-http-field-exception-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: FieldException
---
