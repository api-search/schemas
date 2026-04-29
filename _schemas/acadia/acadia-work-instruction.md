---
description: A digital work instruction document
layout: schema
name: WorkInstruction
properties_list:
- description: Unique work instruction identifier
  name: id
  type: string
- description: Title of the work instruction
  name: title
  type: string
- description: Publication status
  name: status
  type: string
- description: Category or department the instruction belongs to
  name: category
  type: string
- description: Version number of the work instruction
  name: version
  type: integer
- description: Description of the work instruction purpose
  name: description
  type: string
- description: Ordered steps in the work instruction
  name: steps
  type: array
- description: Timestamp when the instruction was created
  name: createdAt
  type: string
- description: Timestamp of last update
  name: updatedAt
  type: string
provider_name: Acadia
provider_slug: acadia
schema_file: json-schema/acadia-work-instruction-schema.json
slug: acadia-work-instruction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-work-instruction-schema.json\",\n  \"title\": \"WorkInstruction\",\n  \"description\": \"A digital work instruction document\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique work instruction identifier\",\n      \"example\": \"wi-abc123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the work instruction\",\n      \"example\": \"Machine Startup Procedure\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Publication status\",\n      \"example\": \"published\",\n      \"enum\": [\n        \"draft\",\n        \"published\",\n        \"archived\"\n      ]\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category or department\
  \ the instruction belongs to\",\n      \"example\": \"operations\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number of the work instruction\",\n      \"example\": 3\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the work instruction purpose\",\n      \"example\": \"Standard procedure for starting production machinery safely\"\n    },\n    \"steps\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered steps in the work instruction\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/WorkInstructionStep\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the instruction was created\",\n      \"example\": \"2026-01-15T09:00:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of last update\"\
  ,\n      \"example\": \"2026-03-01T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-work-instruction-schema.json
tags:
- Connected Worker
- Knowledge Management
- Manufacturing
- Skills Management
- Training
- Workforce Development
title: WorkInstruction
---
