---
description: ''
layout: schema
name: GroupInvitesRequest
properties_list:
- description: ''
  name: invitees
  type: object
- description: ''
  name: message
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-group-invites-request-schema.json
slug: salesforce-group-invites-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"invitees\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"emails\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": \"user@example.com\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\n        \"emails\"\n      ]\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"invitees\",\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupInvitesRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-group-invites-request-schema.json
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
title: GroupInvitesRequest
---
