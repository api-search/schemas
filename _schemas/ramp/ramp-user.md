---
description: Schema describing a user within a Ramp organization.
layout: schema
name: Ramp User
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: first_name
  type: string
- description: ''
  name: last_name
  type: string
- description: ''
  name: role
  type: string
- description: ''
  name: department_id
  type: string
- description: ''
  name: location_id
  type: string
- description: ''
  name: is_manager
  type: boolean
- description: ''
  name: manager_id
  type: string
- description: ''
  name: status
  type: string
provider_name: Ramp
provider_slug: ramp
schema_file: json-schema/ramp-user.json
slug: ramp-user
source_filename: ramp-user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/json-schema/ramp-user.json\",\n  \"title\": \"Ramp User\",\n  \"description\": \"Schema describing a user within a Ramp organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\" },\n    \"email\": { \"type\": \"string\", \"format\": \"email\" },\n    \"first_name\": { \"type\": \"string\" },\n    \"last_name\": { \"type\": \"string\" },\n    \"role\": { \"type\": \"string\", \"enum\": [\"BUSINESS_OWNER\", \"BUSINESS_ADMIN\", \"BUSINESS_USER\", \"BUSINESS_BOOKKEEPER\", \"IT_ADMIN\"] },\n    \"department_id\": { \"type\": \"string\" },\n    \"location_id\": { \"type\": \"string\" },\n    \"is_manager\": { \"type\": \"boolean\" },\n    \"manager_id\": { \"type\": \"string\" },\n    \"status\": { \"type\": \"string\", \"enum\": [\"USER_ACTIVE\", \"USER_SUSPENDED\", \"USER_INACTIVE\"] }\n\
  \  },\n  \"required\": [\"id\", \"email\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/json-schema/ramp-user.json
tags:
- Finance
- Spend Management
- Corporate Cards
- Expense Management
- Accounts Payable
- Bill Pay
- Accounting
- Reimbursements
title: Ramp User
---
