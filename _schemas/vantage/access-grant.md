---
description: An Access Grant that assigns a specific level of access to a Vantage resource for a Team.
layout: schema
name: Vantage Access Grant
properties_list:
- description: The unique token identifier for the Access Grant.
  name: token
  type: string
- description: The token of the Team the grant applies to.
  name: team_token
  type: string
- description: The token of the resource being granted access to.
  name: resource_token
  type: string
- description: The level of access granted.
  name: access
  type: string
- description: The date and time the Access Grant was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/access-grant.json
slug: access-grant
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/access-grant.json\",\n  \"title\": \"Vantage Access Grant\",\n  \"description\": \"An Access Grant that assigns a specific level of access to a Vantage resource for a Team.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Access Grant.\"\n    },\n    \"team_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Team the grant applies to.\"\n    },\n    \"resource_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the resource being granted access to.\"\n    },\n    \"access\": {\n      \"type\": \"string\",\n      \"description\": \"The level of access granted.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"The date and time the Access Grant was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/access-grant.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Access Grant
---
