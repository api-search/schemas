---
description: Response after sending a transactional email
layout: schema
name: TransactionalEmailResponse
properties_list:
- description: The status of the email send
  name: status
  type: string
- description: A unique identifier for tracking the email status
  name: statusId
  type: string
- description: Additional details about the send result
  name: sendResult
  type: string
- description: When the send was requested
  name: requestedAt
  type: string
- description: When the send processing started
  name: startedAt
  type: string
- description: When the send processing completed
  name: completedAt
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/marketing-emal-api-transactional-email-response-schema.json
slug: marketing-emal-api-transactional-email-response
source_filename: marketing-emal-api-transactional-email-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/marketing-emal-api-transactional-email-response-schema.json\",\n  \"title\": \"TransactionalEmailResponse\",\n  \"description\": \"Response after sending a transactional email\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"PROCESSING\",\n        \"CANCELED\",\n        \"COMPLETE\"\n      ],\n      \"description\": \"The status of the email send\",\n      \"example\": \"PENDING\"\n    },\n    \"statusId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for tracking the email status\",\n      \"example\": \"status-id-abc123\"\n    },\n    \"sendResult\": {\n      \"type\": \"string\",\n      \"description\": \"Additional details about the send result\",\n      \"example\": \"SENT\"\n\
  \    },\n    \"requestedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the send was requested\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the send processing started\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the send processing completed\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"statusId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/marketing-emal-api-transactional-email-response-schema.json
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
title: TransactionalEmailResponse
---
