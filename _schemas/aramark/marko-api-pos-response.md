---
description: POSResponse schema from Aramark Marko API
layout: schema
name: POSResponse
properties_list:
- description: ''
  name: data
  type: array
- description: Total record count
  name: count
  type: integer
provider_name: Aramark
provider_slug: aramark
schema_file: json-schema/marko-api-pos-response-schema.json
slug: marko-api-pos-response
source_filename: marko-api-pos-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/POSTransaction\"\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total record count\",\n      \"example\": 100\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-pos-response-schema.json\",\n  \"title\": \"POSResponse\",\n  \"description\": \"POSResponse schema from Aramark Marko API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-pos-response-schema.json
tags:
- Food Services
- Facilities Management
- Uniform Services
- Data Platform
- Fortune 500
title: POSResponse
---
