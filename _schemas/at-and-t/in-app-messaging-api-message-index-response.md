---
description: MessageIndexResponse schema from AT&T API
layout: schema
name: MessageIndexResponse
properties_list:
- description: ''
  name: messageIndexInfo
  type: object
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/in-app-messaging-api-message-index-response-schema.json
slug: in-app-messaging-api-message-index-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/in-app-messaging-api-message-index-response-schema.json\",\n  \"title\": \"MessageIndexResponse\",\n  \"description\": \"MessageIndexResponse schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messageIndexInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"State token to use for delta synchronization\",\n          \"example\": \"state-a1b2c3d4\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Index creation status\",\n          \"enum\": [\n            \"INITIALIZED\",\n            \"IN_PROGRESS\",\n            \"COMPLETE\"\n          ],\n          \"example\": \"INITIALIZED\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/in-app-messaging-api-message-index-response-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: MessageIndexResponse
---
