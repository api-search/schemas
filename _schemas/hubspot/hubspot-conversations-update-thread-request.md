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
schema_file: json-schema/hubspot-conversations-update-thread-request-schema.json
slug: hubspot-conversations-update-thread-request
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request payload for updating a thread's properties.\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"New thread status\",\n      \"example\": \"CLOSED\",\n      \"enum\": [\n        \"OPEN\",\n        \"CLOSED\"\n      ]\n    },\n    \"assignedTo\": {\n      \"type\": \"string\",\n      \"description\": \"User ID to assign the thread to\",\n      \"example\": \"user_789\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateThreadRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-conversations-update-thread-request-schema.json
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
