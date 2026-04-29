---
description: Response for asynchronous action status
layout: schema
name: ActionResponse
properties_list:
- description: Current status of the action
  name: status
  type: string
- description: When the action was requested
  name: requestedAt
  type: string
- description: When the action started processing
  name: startedAt
  type: string
- description: When the action completed
  name: completedAt
  type: string
- description: Related links
  name: links
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/source-code-api-action-response-schema.json
slug: source-code-api-action-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/source-code-api-action-response-schema.json\",\n  \"title\": \"ActionResponse\",\n  \"description\": \"Response for asynchronous action status\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the action\",\n      \"enum\": [\n        \"PENDING\",\n        \"PROCESSING\",\n        \"CANCELED\",\n        \"COMPLETE\"\n      ],\n      \"example\": \"COMPLETE\"\n    },\n    \"requestedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the action was requested\",\n      \"example\": \"2024-01-15T10:30:00Z\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the action started processing\",\n      \"example\"\
  : \"2024-01-15T10:30:01Z\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the action completed\",\n      \"example\": \"2024-01-15T10:30:15Z\"\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Related links\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"startedAt\",\n    \"completedAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/source-code-api-action-response-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: ActionResponse
---
