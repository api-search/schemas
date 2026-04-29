---
description: A User represents an account in Cflow with an assigned role and permissions for accessing workflows.
layout: schema
name: Cflow User
properties_list:
- description: Unique identifier of the user.
  name: id
  type: string
- description: Username of the user.
  name: username
  type: string
- description: Email address of the user.
  name: email
  type: string
- description: Role assigned to the user.
  name: role
  type: string
- description: Account status.
  name: status
  type: string
provider_name: Cflow
provider_slug: cflow
schema_file: json-schema/user.json
slug: user
source_filename: user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cflow/blob/main/json-schema/user.json\",\n  \"title\": \"Cflow User\",\n  \"description\": \"A User represents an account in Cflow with an assigned role and permissions for accessing workflows.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the user.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the user.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Role assigned to the user.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Account status.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\n    \
  \  ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cflow/refs/heads/main/json-schema/user.json
tags:
- Automations
- Business Process Automation
- Integrations
- No-Code
- Platform
- Protocols
- Rules
- Workflows
title: Cflow User
---
