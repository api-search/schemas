---
description: ''
layout: schema
name: Error
properties_list:
- description: ''
  name: message
  type: string
- description: ''
  name: status
  type: integer
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-http-error-schema.json
slug: bloomberg-http-error
source_filename: bloomberg-http-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-http-error-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Error
---
