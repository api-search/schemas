---
description: MessageInput schema
layout: schema
name: MessageInput
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: channel
  type: string
- description: ''
  name: content
  type: object
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/journey-optimizer-api-message-input-schema.json
slug: journey-optimizer-api-message-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-message-input-schema.json\",\n  \"title\": \"MessageInput\",\n  \"description\": \"MessageInput schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"channel\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"email\",\n        \"push\",\n        \"sms\",\n        \"inApp\"\n      ]\n    },\n    \"content\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-message-input-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: MessageInput
---
