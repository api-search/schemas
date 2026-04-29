---
description: Assembly schema from 1Factory API
layout: schema
name: Assembly
properties_list:
- description: ''
  name: part_number
  type: object
- description: ''
  name: rev
  type: object
- description: ''
  name: sub_parts
  type: object
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-assembly-schema.json
slug: 1factory-assembly
source_filename: 1factory-assembly-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-assembly-schema.json\",\n  \"title\": \"Assembly\",\n  \"description\": \"Assembly schema from 1Factory API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"part_number\": {\n      \"$ref\": \"#/components/schemas/part_number\"\n    },\n    \"rev\": {\n      \"$ref\": \"#/components/schemas/rev\"\n    },\n    \"sub_parts\": {\n      \"$ref\": \"#/components/schemas/SubPartList\"\n    }\n  },\n  \"required\": [\n    \"part_number\",\n    \"rev\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-assembly-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: Assembly
---
