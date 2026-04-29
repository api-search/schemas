---
description: A connected SaaS application integration in BetterCloud.
layout: schema
name: Integration
properties_list:
- description: Unique identifier of the integration.
  name: id
  type: string
- description: Display name of the integration.
  name: name
  type: string
- description: Integration type identifier.
  name: type
  type: string
- description: Connection status.
  name: status
  type: string
- description: When the integration was connected.
  name: connected_at
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-integration-schema.json
slug: bettercloud-integration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-integration-schema.json\",\n  \"title\": \"Integration\",\n  \"description\": \"A connected SaaS application integration in BetterCloud.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the integration.\",\n      \"example\": \"int-g001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the integration.\",\n      \"example\": \"Google Workspace\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Integration type identifier.\",\n      \"example\": \"google_workspace\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Connection status.\",\n      \"enum\": [\n        \"connected\",\n        \"disconnected\"\
  ,\n        \"error\"\n      ],\n      \"example\": \"connected\"\n    },\n    \"connected_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"When the integration was connected.\",\n      \"example\": \"2025-01-10T00:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-integration-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: Integration
---
