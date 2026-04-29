---
description: A prime contract for a construction project.
layout: schema
name: Contract
properties_list:
- description: Contract identifier.
  name: id
  type: string
- description: Associated project identifier.
  name: project_id
  type: string
- description: Contract name.
  name: name
  type: string
- description: Contract number.
  name: number
  type: string
- description: Contract status.
  name: status
  type: string
- description: Original contract value in USD.
  name: original_value
  type: number
- description: Revised contract value including change orders.
  name: revised_value
  type: number
- description: Date the contract was executed.
  name: executed_date
  type: string
provider_name: Agave
provider_slug: agave
schema_file: json-schema/unified-api-contract-schema.json
slug: unified-api-contract
source_filename: unified-api-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-contract-schema.json\",\n  \"title\": \"Contract\",\n  \"description\": \"A prime contract for a construction project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Contract identifier.\",\n      \"example\": \"con-778899\"\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated project identifier.\",\n      \"example\": \"proj-500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Contract name.\",\n      \"example\": \"Prime Construction Contract\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Contract number.\",\n      \"example\": \"GC-2025-001\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Contract status.\",\n      \"enum\": [\n        \"draft\",\n        \"approved\",\n        \"executed\",\n        \"completed\",\n        \"voided\"\n      ],\n      \"example\": \"executed\"\n    },\n    \"original_value\": {\n      \"type\": \"number\",\n      \"description\": \"Original contract value in USD.\",\n      \"example\": 4500000.0\n    },\n    \"revised_value\": {\n      \"type\": \"number\",\n      \"description\": \"Revised contract value including change orders.\",\n      \"example\": 4750000.0\n    },\n    \"executed_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the contract was executed.\",\n      \"example\": \"2025-01-20\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-contract-schema.json
tags:
- Accounting
- Construction
- Integration
title: Contract
---
