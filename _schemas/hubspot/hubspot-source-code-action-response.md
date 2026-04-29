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
schema_file: json-schema/hubspot-source-code-action-response-schema.json
slug: hubspot-source-code-action-response
source_filename: hubspot-source-code-action-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response for asynchronous action status\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the action\",\n      \"example\": \"COMPLETE\",\n      \"enum\": [\n        \"PENDING\",\n        \"PROCESSING\",\n        \"CANCELED\",\n        \"COMPLETE\"\n      ]\n    },\n    \"requestedAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the action was requested\",\n      \"format\": \"date-time\",\n      \"example\": \"2024-01-15T10:30:00Z\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the action started processing\",\n      \"format\": \"date-time\",\n      \"example\": \"2024-01-15T10:30:01Z\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the action completed\",\n      \"format\": \"date-time\",\n      \"example\": \"2024-01-15T10:30:15Z\"\n    },\n    \"links\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Related links\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"startedAt\",\n    \"completedAt\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActionResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-source-code-action-response-schema.json
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
