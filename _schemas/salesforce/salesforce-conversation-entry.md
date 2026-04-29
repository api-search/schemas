---
description: ''
layout: schema
name: ConversationEntry
properties_list:
- description: ''
  name: clientDuration
  type: integer
- description: ''
  name: clientTimestamp
  type: integer
- description: ''
  name: identifier
  type: string
- description: ''
  name: messageText
  type: string
- description: ''
  name: relatedRecords
  type: array
- description: ''
  name: sender
  type: object
- description: ''
  name: serverReceivedTimestamp
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-conversation-entry-schema.json
slug: salesforce-conversation-entry
source_filename: salesforce-conversation-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientDuration\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"clientTimestamp\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"messageText\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"relatedRecords\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"sender\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"appType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"role\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"subject\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\
  \n        }\n      },\n      \"required\": [\n        \"appType\",\n        \"role\",\n        \"subject\"\n      ]\n    },\n    \"serverReceivedTimestamp\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"clientDuration\",\n    \"clientTimestamp\",\n    \"identifier\",\n    \"messageText\",\n    \"relatedRecords\",\n    \"sender\",\n    \"serverReceivedTimestamp\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConversationEntry\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-conversation-entry-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: ConversationEntry
---
