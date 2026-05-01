---
description: Contains information about an agent status.
layout: schema
name: AgentStatusSummary
properties_list:
- description: The identifier for an agent status.
  name: Id
  type: string
- description: The Amazon Resource Name (ARN) for the agent status.
  name: Arn
  type: string
- description: The name of the agent status.
  name: Name
  type: string
- description: The type of the agent status.
  name: Type
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/agent-status-summary-schema.json
slug: agent-status-summary
source_filename: agent-status-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/agent-status-summary-schema.json\",\n  \"title\": \"AgentStatusSummary\",\n  \"description\": \"Contains information about an agent status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for an agent status.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-44444EXAMPLE\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the agent status.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the agent status.\",\n      \"example\": \"Available\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the agent status.\",\n      \"enum\": [\n        \"ROUTABLE\",\n        \"CUSTOM\"\
  ,\n        \"OFFLINE\"\n      ],\n      \"example\": \"ROUTABLE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/agent-status-summary-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: AgentStatusSummary
---
