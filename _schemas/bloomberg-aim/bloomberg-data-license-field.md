---
description: ''
layout: schema
name: Field
properties_list:
- description: Bloomberg field mnemonic (e.g., PX_LAST)
  name: identifier
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: description
  type: string
- description: Data type of the field value
  name: dataType
  type: string
- description: ''
  name: category
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-data-license-field-schema.json
slug: bloomberg-data-license-field
source_filename: bloomberg-data-license-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Field\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg field mnemonic (e.g., PX_LAST)\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"description\": \"Data type of the field value\"\n    },\n    \"category\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-data-license-field-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Field
---
