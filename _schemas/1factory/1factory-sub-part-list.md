---
description: List of parts that make up this assembly. Each listed part must already exist as a Part Master entry.
layout: schema
name: SubPartList
properties_list: []
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-sub-part-list-schema.json
slug: 1factory-sub-part-list
source_filename: 1factory-sub-part-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-sub-part-list-schema.json\",\n  \"title\": \"SubPartList\",\n  \"description\": \"List of parts that make up this assembly. Each listed part must already exist as a Part Master entry.\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/AssemblyEntry\"\n  },\n  \"minItems\": 1,\n  \"example\": [\n    {\n      \"part_number\": \"12-54321-21\",\n      \"rev\": \"C\",\n      \"quantity\": 4\n    },\n    {\n      \"part_number\": \"12-54322-11\",\n      \"rev\": \"B\",\n      \"quantity\": 2\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-sub-part-list-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: SubPartList
---
