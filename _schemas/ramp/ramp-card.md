---
description: Schema describing a physical or virtual Ramp card.
layout: schema
name: Ramp Card
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: cardholder_id
  type: string
- description: ''
  name: display_name
  type: string
- description: ''
  name: last_four
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: is_physical
  type: boolean
- description: ''
  name: spending_restrictions
  type: object
provider_name: Ramp
provider_slug: ramp
schema_file: json-schema/ramp-card.json
slug: ramp-card
source_filename: ramp-card.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/json-schema/ramp-card.json\",\n  \"title\": \"Ramp Card\",\n  \"description\": \"Schema describing a physical or virtual Ramp card.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\" },\n    \"cardholder_id\": { \"type\": \"string\" },\n    \"display_name\": { \"type\": \"string\" },\n    \"last_four\": { \"type\": \"string\", \"minLength\": 4, \"maxLength\": 4 },\n    \"state\": { \"type\": \"string\", \"enum\": [\"ACTIVE\", \"SUSPENDED\", \"TERMINATED\", \"UNACTIVATED\"] },\n    \"is_physical\": { \"type\": \"boolean\" },\n    \"spending_restrictions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"amount\": { \"type\": \"number\" },\n        \"interval\": { \"type\": \"string\", \"enum\": [\"DAILY\", \"WEEKLY\", \"MONTHLY\", \"QUARTERLY\", \"YEARLY\", \"TOTAL\"] }\n \
  \     }\n    }\n  },\n  \"required\": [\"id\", \"state\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/json-schema/ramp-card.json
tags:
- Finance
- Spend Management
- Corporate Cards
- Expense Management
- Accounts Payable
- Bill Pay
- Accounting
- Reimbursements
title: Ramp Card
---
