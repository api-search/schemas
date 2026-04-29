---
description: ''
layout: schema
name: Reply
properties_list:
- description: ''
  name: '@type'
  type: string
- description: ''
  name: identifier
  type: string
- description: ''
  name: distributionId
  type: string
- description: ''
  name: contentType
  type: string
- description: Size in bytes
  name: size
  type: integer
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-data-license-reply-schema.json
slug: bloomberg-data-license-reply
source_filename: bloomberg-data-license-reply-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Reply\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\"\n    },\n    \"identifier\": {\n      \"type\": \"string\"\n    },\n    \"distributionId\": {\n      \"type\": \"string\"\n    },\n    \"contentType\": {\n      \"type\": \"string\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Size in bytes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-data-license-reply-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Reply
---
