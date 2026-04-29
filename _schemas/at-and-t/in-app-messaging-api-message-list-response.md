---
description: MessageListResponse schema from AT&T API
layout: schema
name: MessageListResponse
properties_list:
- description: ''
  name: messageResultSet
  type: object
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/in-app-messaging-api-message-list-response-schema.json
slug: in-app-messaging-api-message-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/in-app-messaging-api-message-list-response-schema.json\",\n  \"title\": \"MessageListResponse\",\n  \"description\": \"MessageListResponse schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messageResultSet\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"messages\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"messageId\": {\n                \"type\": \"string\",\n                \"description\": \"Unique message identifier\",\n                \"example\": \"msg-500123\"\n              },\n              \"from\": {\n                \"type\": \"string\",\n                \"description\": \"Sender address (phone number or email)\",\n                \"example\": \"tel:+12125551234\"\
  \n              },\n              \"recipients\": {\n                \"type\": \"array\",\n                \"description\": \"List of recipient addresses\",\n                \"items\": {\n                  \"type\": \"string\"\n                },\n                \"example\": [\n                  \"tel:+12125559999\"\n                ]\n              },\n              \"isUnread\": {\n                \"type\": \"boolean\",\n                \"description\": \"Whether the message has been read\",\n                \"example\": false\n              },\n              \"isIncoming\": {\n                \"type\": \"boolean\",\n                \"description\": \"True if message was received, false if sent\",\n                \"example\": true\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"Message type\",\n                \"enum\": [\n                  \"TEXT\",\n                  \"MMS\"\n                ],\n            \
  \    \"example\": \"TEXT\"\n              },\n              \"typeCode\": {\n                \"type\": \"string\",\n                \"description\": \"Numeric type code\",\n                \"example\": \"1\"\n              },\n              \"timeStamp\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\",\n                \"description\": \"Date and time the message was sent or received\",\n                \"example\": \"2026-04-19T14:30:00Z\"\n              }\n            }\n          }\n        },\n        \"totalCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of messages matching the query\",\n          \"example\": 1\n        },\n        \"offset\": {\n          \"type\": \"integer\",\n          \"description\": \"Current pagination offset\",\n          \"example\": 0\n        },\n        \"limit\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum messages per page\",\n          \"example\"\
  : 50\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/in-app-messaging-api-message-list-response-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: MessageListResponse
---
