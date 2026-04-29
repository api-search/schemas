---
description: A historical property value
layout: schema
name: PropertyHistory
properties_list:
- description: The property value
  name: value
  type: string
- description: When this value was set
  name: timestamp
  type: string
- description: The source that set this value
  name: sourceType
  type: string
- description: The identifier of the source
  name: sourceId
  type: string
- description: A human-readable label for the source
  name: sourceLabel
  type: string
- description: The user ID that made the change
  name: updatedByUserId
  type: integer
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-commerce-payments-property-history-schema.json
slug: hubspot-commerce-payments-property-history
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A historical property value\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The property value\",\n      \"example\": \"example-value\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"When this value was set\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"sourceType\": {\n      \"type\": \"string\",\n      \"description\": \"The source that set this value\",\n      \"example\": \"standard\"\n    },\n    \"sourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the source\",\n      \"example\": \"500123\"\n    },\n    \"sourceLabel\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable label for the source\",\n      \"example\": \"Example Record\"\n    },\n    \"updatedByUserId\": {\n      \"type\": \"integer\",\n      \"description\": \"The\
  \ user ID that made the change\",\n      \"example\": 1718153645993\n    }\n  },\n  \"required\": [\n    \"value\",\n    \"timestamp\",\n    \"sourceType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PropertyHistory\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-commerce-payments-property-history-schema.json
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
