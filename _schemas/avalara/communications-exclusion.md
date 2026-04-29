---
description: Exclusion schema from Avalara API
layout: schema
name: Exclusion
properties_list:
- description: Exclusion type
  name: excl
  type: integer
- description: ''
  name: ctry
  type: string
- description: ''
  name: st
  type: string
- description: ''
  name: excl_name
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-exclusion-schema.json
slug: communications-exclusion
source_filename: communications-exclusion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-exclusion-schema.json\",\n  \"title\": \"Exclusion\",\n  \"description\": \"Exclusion schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"excl\": {\n      \"type\": \"integer\",\n      \"description\": \"Exclusion type\"\n    },\n    \"ctry\": {\n      \"type\": \"string\"\n    },\n    \"st\": {\n      \"type\": \"string\"\n    },\n    \"excl_name\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-exclusion-schema.json
tags:
- Taxes
title: Exclusion
---
