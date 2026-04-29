---
description: A budget line item for a construction project.
layout: schema
name: Budget
properties_list:
- description: Agave budget line item identifier.
  name: id
  type: string
- description: Associated project identifier.
  name: project_id
  type: string
- description: Associated cost code identifier.
  name: cost_code_id
  type: string
- description: Budget line item description.
  name: description
  type: string
- description: Original budgeted amount in USD.
  name: original_amount
  type: number
- description: Revised budget amount including changes.
  name: revised_amount
  type: number
- description: Actual cost incurred to date.
  name: actual_cost
  type: number
- description: Total projected cost at completion.
  name: projected_cost
  type: number
provider_name: Agave
provider_slug: agave
schema_file: json-schema/unified-api-budget-schema.json
slug: unified-api-budget
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-budget-schema.json\",\n  \"title\": \"Budget\",\n  \"description\": \"A budget line item for a construction project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Agave budget line item identifier.\",\n      \"example\": \"bud-112233\"\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated project identifier.\",\n      \"example\": \"proj-500123\"\n    },\n    \"cost_code_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated cost code identifier.\",\n      \"example\": \"cc-445566\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Budget line item description.\",\n      \"example\": \"Concrete Foundation Work\"\n    },\n    \"original_amount\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"Original budgeted amount in USD.\",\n      \"example\": 250000.0\n    },\n    \"revised_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Revised budget amount including changes.\",\n      \"example\": 275000.0\n    },\n    \"actual_cost\": {\n      \"type\": \"number\",\n      \"description\": \"Actual cost incurred to date.\",\n      \"example\": 180000.0\n    },\n    \"projected_cost\": {\n      \"type\": \"number\",\n      \"description\": \"Total projected cost at completion.\",\n      \"example\": 270000.0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-budget-schema.json
tags:
- Accounting
- Construction
- Integration
title: Budget
---
