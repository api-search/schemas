---
description: Represents a usage event for an application, capturing user actions such as starting a video call, sending messages, or uploading files.
layout: schema
name: UsageEvent
properties_list:
- description: The timestamp of the event in milliseconds since epoch.
  name: timestamp
  type: integer
- description: The email address of the user who performed the action.
  name: email
  type: string
- description: The name of the action or activity performed.
  name: eventName
  type: string
provider_name: Productiv
provider_slug: productiv
schema_file: json-schema/usage-event.json
slug: usage-event
source_json: "{\n  \"$id\": \"usage-event.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UsageEvent\",\n  \"description\": \"Represents a usage event for an application, capturing user actions such as starting a video call, sending messages, or uploading files.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"timestamp\",\n    \"email\",\n    \"eventName\"\n  ],\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"The timestamp of the event in milliseconds since epoch.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the user who performed the action.\"\n    },\n    \"eventName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the action or activity performed.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/json-schema/usage-event.json
tags:
- Application Portfolio
- Provisioning
- SaaS Management
- Spend Management
- Usage Analytics
title: UsageEvent
---
