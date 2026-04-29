---
description: SendMessageRequest schema from AT&T API
layout: schema
name: SendMessageRequest
properties_list:
- description: ''
  name: messageRequest
  type: object
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/in-app-messaging-api-send-message-request-schema.json
slug: in-app-messaging-api-send-message-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/in-app-messaging-api-send-message-request-schema.json\",\n  \"title\": \"SendMessageRequest\",\n  \"description\": \"SendMessageRequest schema from AT&T API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"messageRequest\"\n  ],\n  \"properties\": {\n    \"messageRequest\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"addresses\"\n      ],\n      \"properties\": {\n        \"addresses\": {\n          \"type\": \"array\",\n          \"description\": \"List of recipient phone numbers or email addresses\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"example\": [\n            \"tel:+12125551234\"\n          ]\n        },\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"SMS text content (up to 160 chars for SMS, longer\
  \ for MMS)\",\n          \"example\": \"Hello from the AT&T In-App Messaging API!\"\n        },\n        \"subject\": {\n          \"type\": \"string\",\n          \"description\": \"Subject line (MMS only)\",\n          \"example\": \"Greeting\"\n        },\n        \"group\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, send as a group message\",\n          \"example\": false\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/in-app-messaging-api-send-message-request-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: SendMessageRequest
---
