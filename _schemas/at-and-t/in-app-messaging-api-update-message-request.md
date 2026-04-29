---
description: UpdateMessageRequest schema from AT&T API
layout: schema
name: UpdateMessageRequest
properties_list:
- description: ''
  name: message
  type: object
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/in-app-messaging-api-update-message-request-schema.json
slug: in-app-messaging-api-update-message-request
source_filename: in-app-messaging-api-update-message-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/in-app-messaging-api-update-message-request-schema.json\",\n  \"title\": \"UpdateMessageRequest\",\n  \"description\": \"UpdateMessageRequest schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"isUnread\": {\n          \"type\": \"boolean\",\n          \"description\": \"Updated read status of the message\",\n          \"example\": false\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/in-app-messaging-api-update-message-request-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: UpdateMessageRequest
---
