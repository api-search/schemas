---
description: InboundSmsResponse schema from AT&T API
layout: schema
name: InboundSmsResponse
properties_list:
- description: ''
  name: inboundSMSMessageList
  type: object
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/sms-api-inbound-sms-response-schema.json
slug: sms-api-inbound-sms-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-inbound-sms-response-schema.json\",\n  \"title\": \"InboundSmsResponse\",\n  \"description\": \"InboundSmsResponse schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inboundSMSMessageList\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"inboundSMSMessage\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"messageId\": {\n                \"type\": \"string\",\n                \"description\": \"Unique identifier for the inbound message\",\n                \"example\": \"msg-500456\"\n              },\n              \"message\": {\n                \"type\": \"string\",\n                \"description\": \"SMS message text content\",\n                \"example\": \"STOP\"\
  \n              },\n              \"senderAddress\": {\n                \"type\": \"string\",\n                \"description\": \"Phone number of the message sender in tel:+E.164 format\",\n                \"example\": \"tel:+12125551234\"\n              },\n              \"destinationAddress\": {\n                \"type\": \"string\",\n                \"description\": \"Short code that received the message\",\n                \"example\": \"12345\"\n              },\n              \"dateTime\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\",\n                \"description\": \"Date and time when the message was received\",\n                \"example\": \"2026-04-19T14:30:00Z\"\n              }\n            }\n          }\n        },\n        \"numberOfMessagesInThisBatch\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of messages in this response batch\",\n          \"example\": 1\n        },\n        \"resourceURL\": {\n\
  \          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of this inbox resource\",\n          \"example\": \"https://api.att.com/sms/v3/messaging/inbox/REG-500123\"\n        },\n        \"totalNumberOfPendingMessages\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of messages waiting to be retrieved\",\n          \"example\": 0\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-inbound-sms-response-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: InboundSmsResponse
---
