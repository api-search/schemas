---
description: Paginated list of work instructions
layout: schema
name: WorkInstructionList
properties_list:
- description: ''
  name: data
  type: array
- description: Total number of work instructions
  name: total
  type: integer
- description: Current page number
  name: page
  type: integer
- description: Results per page
  name: limit
  type: integer
provider_name: Acadia
provider_slug: acadia
schema_file: json-schema/acadia-work-instruction-list-schema.json
slug: acadia-work-instruction-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-work-instruction-list-schema.json\",\n  \"title\": \"WorkInstructionList\",\n  \"description\": \"Paginated list of work instructions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/WorkInstruction\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of work instructions\",\n      \"example\": 42\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number\",\n      \"example\": 1\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Results per page\",\n      \"example\": 25\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-work-instruction-list-schema.json
tags:
- Connected Worker
- Knowledge Management
- Manufacturing
- Skills Management
- Training
- Workforce Development
title: WorkInstructionList
---
