---
description: ''
layout: schema
name: FieldInfoRequest
properties_list:
- description: List of field mnemonics or IDs to look up
  name: fieldId
  type: array
- description: ''
  name: returnFieldDocumentation
  type: boolean
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-http-field-info-request-schema.json
slug: bloomberg-http-field-info-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FieldInfoRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldId\": {\n      \"type\": \"array\",\n      \"description\": \"List of field mnemonics or IDs to look up\"\n    },\n    \"returnFieldDocumentation\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-http-field-info-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: FieldInfoRequest
---
