---
description: Delivery status information for a message
layout: schema
name: MessageStatus
properties_list:
- description: Current delivery status type
  name: statusType
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/conversations-api-message-status-schema.json
slug: conversations-api-message-status
source_filename: conversations-api-message-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-message-status-schema.json\",\n  \"title\": \"MessageStatus\",\n  \"description\": \"Delivery status information for a message\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SENT\",\n        \"DELIVERED\",\n        \"READ\",\n        \"FAILED\"\n      ],\n      \"description\": \"Current delivery status type\",\n      \"example\": \"DELIVERED\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-message-status-schema.json
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
title: MessageStatus
---
