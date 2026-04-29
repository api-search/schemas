---
description: UpdateUserRequest schema from Activepieces API
layout: schema
name: UpdateUserRequest
properties_list:
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: platformRole
  type: string
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-update-user-request-schema.json
slug: activepieces-update-user-request
source_filename: activepieces-update-user-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-update-user-request-schema.json\",\n  \"title\": \"UpdateUserRequest\",\n  \"description\": \"UpdateUserRequest schema from Activepieces API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"platformRole\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ADMIN\",\n        \"MEMBER\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-update-user-request-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: UpdateUserRequest
---
