---
description: Request body for creating a new end user
layout: schema
name: CreateUserRequest
properties_list:
- description: Unique username or external identifier
  name: username
  type: string
- description: Full display name of the user
  name: fullName
  type: string
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-embedded-create_user_request-schema.json
slug: alloy-embedded-create_user_request
source_filename: alloy-embedded-create_user_request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-embedded-create_user_request-schema.json\",\n  \"title\": \"CreateUserRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new end user\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Unique username or external identifier\"\n    },\n    \"fullName\": {\n      \"type\": \"string\",\n      \"description\": \"Full display name of the user\"\n    }\n  },\n  \"required\": [\n    \"username\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-embedded-create_user_request-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: CreateUserRequest
---
