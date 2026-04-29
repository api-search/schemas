---
description: ''
layout: schema
name: RegisterFieldWKTRequest
properties_list:
- description: ''
  name: wkt
  type: string
- description: Percentage overlap threshold
  name: threshold
  type: integer
- description: ''
  name: return_s2_indices
  type: boolean
- description: Comma-separated list of resolution levels
  name: s2_index
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-asset-registry-registerfieldwktrequest-schema.json
slug: agstack-asset-registry-registerfieldwktrequest
source_filename: agstack-asset-registry-registerfieldwktrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/RegisterFieldWKTRequest.json\",\n  \"title\": \"RegisterFieldWKTRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"wkt\"\n  ],\n  \"properties\": {\n    \"wkt\": {\n      \"type\": \"string\",\n      \"example\": \"POLYGON((75.78209 30.90706, 75.78211 30.90645, 75.78270 30.90654, 75.78262 30.90714, 75.78209 30.90706))\"\n    },\n    \"threshold\": {\n      \"type\": \"integer\",\n      \"default\": 95,\n      \"description\": \"Percentage overlap threshold\"\n    },\n    \"return_s2_indices\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"s2_index\": {\n      \"type\": \"string\",\n      \"example\": \"8,13\",\n      \"description\": \"Comma-separated list of resolution levels\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-asset-registry-registerfieldwktrequest-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: RegisterFieldWKTRequest
---
