---
description: A user in the Alloy Connectivity platform
layout: schema
name: User
properties_list:
- description: Unique identifier for the user
  name: userId
  type: string
- description: Username or external identifier
  name: username
  type: string
- description: Timestamp when the user was created
  name: createdAt
  type: string
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-user-schema.json
slug: alloy-connectivity-user
source_filename: alloy-connectivity-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-user-schema.json\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"description\": \"A user in the Alloy Connectivity platform\",\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Username or external identifier\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the user was created\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-user-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: User
---
