---
description: SendMessageResponse schema from AT&T API
layout: schema
name: SendMessageResponse
properties_list:
- description: Unique identifier for the sent message
  name: id
  type: string
- description: URL to access the message resource
  name: resourceURL
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/in-app-messaging-api-send-message-response-schema.json
slug: in-app-messaging-api-send-message-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/in-app-messaging-api-send-message-response-schema.json\",\n  \"title\": \"SendMessageResponse\",\n  \"description\": \"SendMessageResponse schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the sent message\",\n      \"example\": \"msg-500123\"\n    },\n    \"resourceURL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to access the message resource\",\n      \"example\": \"https://api.att.com/myMessages/v2/messages/msg-500123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/in-app-messaging-api-send-message-response-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: SendMessageResponse
---
