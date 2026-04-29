---
description: ''
layout: schema
name: AccountResult
properties_list:
- description: Account holder first name.
  name: first_name
  type: string
- description: Account holder last name.
  name: last_name
  type: string
- description: Account email address.
  name: email
  type: string
- description: Name of the current subscription plan.
  name: plan_name
  type: string
- description: Level of the current subscription plan.
  name: plan_level
  type: integer
- description: Date when usage counters reset.
  name: reset_date
  type: string
- description: Team identifier.
  name: team_id
  type: integer
- description: Usage breakdown by request type.
  name: requests
  type: object
- description: Deprecated. Total usage counters.
  name: calls
  type: object
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-account-result-schema.json
slug: hunter-account-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"Account holder first name.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Account holder last name.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Account email address.\"\n    },\n    \"plan_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the current subscription plan.\"\n    },\n    \"plan_level\": {\n      \"type\": \"integer\",\n      \"description\": \"Level of the current subscription plan.\"\n    },\n    \"reset_date\": {\n      \"type\": \"string\",\n      \"description\": \"Date when usage counters reset.\"\n    },\n    \"team_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Team identifier.\"\n    },\n    \"requests\": {\n      \"\
  type\": \"object\",\n      \"description\": \"Usage breakdown by request type.\"\n    },\n    \"calls\": {\n      \"type\": \"object\",\n      \"description\": \"Deprecated. Total usage counters.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-account-result-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: AccountResult
---
