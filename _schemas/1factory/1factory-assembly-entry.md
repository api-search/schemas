---
description: AssemblyEntry schema from 1Factory API
layout: schema
name: AssemblyEntry
properties_list:
- description: ''
  name: part_number
  type: object
- description: ''
  name: rev
  type: object
- description: Number of instances of this part in the assembly.
  name: quantity
  type: number
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-assembly-entry-schema.json
slug: 1factory-assembly-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-assembly-entry-schema.json\",\n  \"title\": \"AssemblyEntry\",\n  \"description\": \"AssemblyEntry schema from 1Factory API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"part_number\": {\n      \"$ref\": \"#/components/schemas/part_number\"\n    },\n    \"rev\": {\n      \"$ref\": \"#/components/schemas/rev\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"nullable\": false,\n      \"minimum\": 0,\n      \"description\": \"Number of instances of this part in the assembly.\",\n      \"example\": 4.0\n    }\n  },\n  \"required\": [\n    \"part_number\",\n    \"rev\",\n    \"quantity\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-assembly-entry-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: AssemblyEntry
---
