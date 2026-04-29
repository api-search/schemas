---
description: SendSmsResponse schema from AT&T API
layout: schema
name: SendSmsResponse
properties_list:
- description: ''
  name: outboundSMSResponse
  type: object
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/sms-api-send-sms-response-schema.json
slug: sms-api-send-sms-response
source_filename: sms-api-send-sms-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-send-sms-response-schema.json\",\n  \"title\": \"SendSmsResponse\",\n  \"description\": \"SendSmsResponse schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"outboundSMSResponse\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"messageId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the sent message\",\n          \"example\": \"msg-500123\"\n        },\n        \"resourceReference\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"resourceURL\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"URL to check delivery status of this message\",\n              \"example\": \"https://api.att.com/sms/v3/messaging/outbox/msg-500123\"\
  \n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-send-sms-response-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: SendSmsResponse
---
