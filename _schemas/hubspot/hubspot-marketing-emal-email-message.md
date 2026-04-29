---
description: The email message configuration
layout: schema
name: EmailMessage
properties_list:
- description: The recipient's email address
  name: to
  type: string
- description: Override the from address (must be verified)
  name: from
  type: string
- description: A unique ID to prevent duplicate sends
  name: sendId
  type: string
- description: Reply-to email addresses
  name: replyTo
  type: array
- description: CC email addresses
  name: cc
  type: array
- description: BCC email addresses
  name: bcc
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-marketing-emal-email-message-schema.json
slug: hubspot-marketing-emal-email-message
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The email message configuration\",\n  \"properties\": {\n    \"to\": {\n      \"type\": \"string\",\n      \"description\": \"The recipient's email address\",\n      \"format\": \"email\",\n      \"example\": \"recipient@example.com\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"Override the from address (must be verified)\",\n      \"format\": \"email\",\n      \"example\": \"noreply@yourcompany.com\"\n    },\n    \"sendId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique ID to prevent duplicate sends\",\n      \"example\": \"unique-send-id-123\"\n    },\n    \"replyTo\": {\n      \"type\": \"array\",\n      \"description\": \"Reply-to email addresses\",\n      \"example\": [\n        \"support@yourcompany.com\"\n      ],\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"email\"\n      }\n    },\n    \"cc\": {\n      \"type\": \"array\",\n      \"\
  description\": \"CC email addresses\",\n      \"example\": [\n        \"jsmith@example.com\"\n      ],\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"email\"\n      }\n    },\n    \"bcc\": {\n      \"type\": \"array\",\n      \"description\": \"BCC email addresses\",\n      \"example\": [\n        \"jsmith@example.com\"\n      ],\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"email\"\n      }\n    }\n  },\n  \"required\": [\n    \"to\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-marketing-emal-email-message-schema.json
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
title: EmailMessage
---
