---
description: A job cost code for categorizing construction costs.
layout: schema
name: CostCode
properties_list:
- description: Cost code identifier.
  name: id
  type: string
- description: Associated project identifier.
  name: project_id
  type: string
- description: Cost code value.
  name: code
  type: string
- description: Cost code description.
  name: description
  type: string
- description: Cost type classification.
  name: cost_type
  type: string
provider_name: Agave
provider_slug: agave
schema_file: json-schema/unified-api-cost-code-schema.json
slug: unified-api-cost-code
source_filename: unified-api-cost-code-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-cost-code-schema.json\",\n  \"title\": \"CostCode\",\n  \"description\": \"A job cost code for categorizing construction costs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Cost code identifier.\",\n      \"example\": \"cc-445566\"\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated project identifier.\",\n      \"example\": \"proj-500123\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Cost code value.\",\n      \"example\": \"03-1000\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Cost code description.\",\n      \"example\": \"Concrete\"\n    },\n    \"cost_type\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Cost type classification.\",\n      \"enum\": [\n        \"labor\",\n        \"material\",\n        \"equipment\",\n        \"subcontract\",\n        \"other\"\n      ],\n      \"example\": \"material\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-cost-code-schema.json
tags:
- Accounting
- Construction
- Integration
title: CostCode
---
