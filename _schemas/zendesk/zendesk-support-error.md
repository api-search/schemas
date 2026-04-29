---
description: An error response from the Zendesk API.
layout: schema
name: Error
properties_list:
- description: The error type identifier.
  name: error
  type: string
- description: A human-readable description of the error.
  name: description
  type: string
- description: Additional details about the error.
  name: details
  type: object
provider_name: Zendesk
provider_slug: zendesk
schema_file: json-schema/zendesk-support-error-schema.json
slug: zendesk-support-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"An error response from the Zendesk API.\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"The error type identifier.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the error.\"\n    },\n    \"details\": {\n      \"type\": \"object\",\n      \"description\": \"Additional details about the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-support-error-schema.json
tags:
- Chat
- CRM
- Help Center
- Sell
- Support
- T1
- Talk
- Ticketing
- Tickets
title: Error
---
