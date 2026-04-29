---
description: Represents a call engagement in the CRM
layout: schema
name: Call
properties_list:
- description: The unique identifier for the call
  name: id
  type: string
- description: The call properties
  name: properties
  type: object
- description: Properties with their change history
  name: propertiesWithHistory
  type: object
- description: When the call was created
  name: createdAt
  type: string
- description: When the call was last updated
  name: updatedAt
  type: string
- description: Whether the call is archived
  name: archived
  type: boolean
- description: When the call was archived (if archived)
  name: archivedAt
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-calls-call-schema.json
slug: hubspot-engagement-calls-call
source_filename: hubspot-engagement-calls-call-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Represents a call engagement in the CRM\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the call\",\n      \"example\": \"512\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The call properties\",\n      \"example\": {\n        \"hs_call_title\": \"Discovery Call\",\n        \"hs_call_body\": \"Discussed product requirements\",\n        \"hs_call_duration\": \"1800000\",\n        \"hs_call_direction\": \"OUTBOUND\",\n        \"hs_call_disposition\": \"connected\",\n        \"hs_call_status\": \"COMPLETED\",\n        \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\"\n      }\n    },\n    \"propertiesWithHistory\": {\n      \"type\": \"object\",\n      \"description\": \"Properties with their change history\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"When the call was created\",\n      \"format\": \"date-time\",\n      \"example\": \"2024-01-15T10:30:00.000Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the call was last updated\",\n      \"format\": \"date-time\",\n      \"example\": \"2024-01-15T11:00:00.000Z\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the call is archived\",\n      \"example\": false\n    },\n    \"archivedAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the call was archived (if archived)\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"properties\",\n    \"createdAt\",\n    \"updatedAt\",\n    \"archived\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Call\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-calls-call-schema.json
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
title: Call
---
