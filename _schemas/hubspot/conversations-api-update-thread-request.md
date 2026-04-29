---
description: Request payload for updating a thread's properties.
layout: schema
name: UpdateThreadRequest
properties_list:
- description: New thread status
  name: status
  type: string
- description: User ID to assign the thread to
  name: assignedTo
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/conversations-api-update-thread-request-schema.json
slug: conversations-api-update-thread-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-update-thread-request-schema.json\",\n  \"title\": \"UpdateThreadRequest\",\n  \"description\": \"Request payload for updating a thread's properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OPEN\",\n        \"CLOSED\"\n      ],\n      \"description\": \"New thread status\",\n      \"example\": \"CLOSED\"\n    },\n    \"assignedTo\": {\n      \"type\": \"string\",\n      \"description\": \"User ID to assign the thread to\",\n      \"example\": \"user_789\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-update-thread-request-schema.json
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
title: UpdateThreadRequest
---
