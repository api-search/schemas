---
description: ''
layout: schema
name: SecurityIdentifier
properties_list:
- description: ''
  name: '@type'
  type: string
- description: Type of identifier
  name: identifierType
  type: string
- description: The identifier value
  name: identifierValue
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-data-license-security-identifier-schema.json
slug: bloomberg-data-license-security-identifier
source_filename: bloomberg-data-license-security-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecurityIdentifier\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\"\n    },\n    \"identifierType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of identifier\"\n    },\n    \"identifierValue\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-data-license-security-identifier-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: SecurityIdentifier
---
