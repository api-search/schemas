---
description: ''
layout: schema
name: Catalog
properties_list:
- description: Unique catalog identifier
  name: identifier
  type: string
- description: Human-readable catalog title
  name: title
  type: string
- description: Description of the catalog contents
  name: description
  type: string
- description: ''
  name: links
  type: object
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-data-license-catalog-schema.json
slug: bloomberg-data-license-catalog
source_filename: bloomberg-data-license-catalog-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Catalog\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Unique catalog identifier\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable catalog title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the catalog contents\"\n    },\n    \"links\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-data-license-catalog-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Catalog
---
