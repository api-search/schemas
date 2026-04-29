---
description: Historical value of a property
layout: schema
name: PropertyHistory
properties_list:
- description: The historical value
  name: value
  type: string
- description: When the value was set
  name: timestamp
  type: string
- description: The source type that set this value
  name: sourceType
  type: string
- description: The source identifier
  name: sourceId
  type: string
- description: Human-readable source label
  name: sourceLabel
  type: string
- description: The user ID who made the change
  name: updatedByUserId
  type: integer
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-calls-api-property-history-schema.json
slug: engagement-calls-api-property-history
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-property-history-schema.json\",\n  \"title\": \"PropertyHistory\",\n  \"description\": \"Historical value of a property\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The historical value\",\n      \"example\": \"Discovery Call\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the value was set\",\n      \"example\": \"2024-01-15T10:30:00.000Z\"\n    },\n    \"sourceType\": {\n      \"type\": \"string\",\n      \"description\": \"The source type that set this value\",\n      \"example\": \"CRM_UI\"\n    },\n    \"sourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The source identifier\",\n      \"example\": \"userId:12345\"\
  \n    },\n    \"sourceLabel\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable source label\",\n      \"example\": \"John Doe\"\n    },\n    \"updatedByUserId\": {\n      \"type\": \"integer\",\n      \"description\": \"The user ID who made the change\",\n      \"example\": 12345\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-property-history-schema.json
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
title: PropertyHistory
---
