---
description: ''
layout: schema
name: Error
properties_list:
- description: ''
  name: STATUS
  type: integer
- description: ''
  name: MESSAGE
  type: string
- description: ''
  name: REASON
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-error-schema.json
slug: bloomberg-emsx-error
source_filename: bloomberg-emsx-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"STATUS\": {\n      \"type\": \"integer\"\n    },\n    \"MESSAGE\": {\n      \"type\": \"string\"\n    },\n    \"REASON\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-error-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Error
---
