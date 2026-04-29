---
description: ''
layout: schema
name: Override
properties_list:
- description: Bloomberg field mnemonic to override
  name: fieldId
  type: string
- description: Override value
  name: value
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-http-override-schema.json
slug: bloomberg-http-override
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Override\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldId\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg field mnemonic to override\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Override value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-http-override-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Override
---
