---
description: SendSmsRequest schema from AT&T API
layout: schema
name: SendSmsRequest
properties_list:
- description: ''
  name: outboundSMSRequest
  type: object
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/sms-api-send-sms-request-schema.json
slug: sms-api-send-sms-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-send-sms-request-schema.json\",\n  \"title\": \"SendSmsRequest\",\n  \"description\": \"SendSmsRequest schema from AT&T API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"outboundSMSRequest\"\n  ],\n  \"properties\": {\n    \"outboundSMSRequest\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"address\",\n        \"message\"\n      ],\n      \"properties\": {\n        \"address\": {\n          \"type\": \"array\",\n          \"description\": \"List of destination phone numbers in tel:+E.164 format (max 50)\",\n          \"items\": {\n            \"type\": \"string\",\n            \"example\": \"tel:+12125551234\"\n          },\n          \"example\": [\n            \"tel:+12125551234\"\n          ]\n        },\n        \"message\": {\n          \"type\": \"string\",\n        \
  \  \"description\": \"SMS message text (max 4096 characters)\",\n          \"example\": \"Your verification code is 482910. Valid for 10 minutes.\"\n        },\n        \"notifyDeliveryStatus\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, delivery status notifications are sent to the registered callback URL\",\n          \"example\": true\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-send-sms-request-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: SendSmsRequest
---
