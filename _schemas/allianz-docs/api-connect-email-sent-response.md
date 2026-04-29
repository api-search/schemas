---
description: Confirmation that an email has been sent
layout: schema
name: EmailSentResponse
properties_list:
- description: Unique identifier for the sent message
  name: message_id
  type: string
- description: Status of the email delivery
  name: status
  type: string
- description: Timestamp when the email was sent
  name: sent_at
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-email-sent-response-schema.json
slug: api-connect-email-sent-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-email-sent-response-schema.json\",\n  \"title\": \"EmailSentResponse\",\n  \"description\": \"Confirmation that an email has been sent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the sent message\",\n      \"example\": \"msg-500456\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the email delivery\",\n      \"enum\": [\n        \"sent\",\n        \"pending\",\n        \"failed\"\n      ],\n      \"example\": \"sent\"\n    },\n    \"sent_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the email was sent\",\n      \"example\": \"2026-04-19T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-email-sent-response-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: EmailSentResponse
---
