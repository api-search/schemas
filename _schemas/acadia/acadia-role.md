---
description: A job role with training requirements
layout: schema
name: Role
properties_list:
- description: Role identifier
  name: id
  type: string
- description: Role name
  name: name
  type: string
- description: Department the role belongs to
  name: department
  type: string
- description: Number of required training completions for the role
  name: requiredTrainings
  type: integer
- description: Average completion rate across employees in this role
  name: completionRate
  type: integer
provider_name: Acadia
provider_slug: acadia
schema_file: json-schema/acadia-role-schema.json
slug: acadia-role
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-role-schema.json\",\n  \"title\": \"Role\",\n  \"description\": \"A job role with training requirements\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Role identifier\",\n      \"example\": \"role-ops-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Role name\",\n      \"example\": \"Machine Operator\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Department the role belongs to\",\n      \"example\": \"Production\"\n    },\n    \"requiredTrainings\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of required training completions for the role\",\n      \"example\": 12\n    },\n    \"completionRate\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"Average completion rate across employees in this role\",\n      \"example\": 78\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-role-schema.json
tags:
- Connected Worker
- Knowledge Management
- Manufacturing
- Skills Management
- Training
- Workforce Development
title: Role
---
