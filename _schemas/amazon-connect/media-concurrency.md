---
description: Contains information about which channels are supported, and how many contacts an agent can have on a channel simultaneously.
layout: schema
name: MediaConcurrency
properties_list:
- description: The channels that agents can handle in the Contact Control Panel (CCP).
  name: Channel
  type: string
- description: The number of contacts an agent can have on a channel simultaneously.
  name: Concurrency
  type: integer
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/media-concurrency-schema.json
slug: media-concurrency
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/media-concurrency-schema.json\",\n  \"title\": \"MediaConcurrency\",\n  \"description\": \"Contains information about which channels are supported, and how many contacts an agent can have on a channel simultaneously.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Channel\": {\n      \"type\": \"string\",\n      \"description\": \"The channels that agents can handle in the Contact Control Panel (CCP).\",\n      \"enum\": [\n        \"VOICE\",\n        \"CHAT\",\n        \"TASK\",\n        \"EMAIL\"\n      ],\n      \"example\": \"VOICE\"\n    },\n    \"Concurrency\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of contacts an agent can have on a channel simultaneously.\",\n      \"minimum\": 1,\n      \"maximum\": 10,\n      \"example\": 1\n    }\n  },\n  \"required\": [\n\
  \    \"Channel\",\n    \"Concurrency\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/media-concurrency-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: MediaConcurrency
---
