---
description: Request to send an SMS via AT&T Wireless APIs
layout: schema
name: Send SMS Request
properties_list:
- description: ''
  name: outboundSMSRequest
  type: object
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/wireless-apis-send-sms-request-schema.json
slug: wireless-apis-send-sms-request
source_filename: wireless-apis-send-sms-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.att.com/schemas/wireless/send-sms-request\",\n  \"title\": \"Send SMS Request\",\n  \"description\": \"Request to send an SMS via AT&T Wireless APIs\",\n  \"type\": \"object\",\n  \"required\": [\n    \"outboundSMSRequest\"\n  ],\n  \"properties\": {\n    \"outboundSMSRequest\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"address\",\n        \"message\"\n      ],\n      \"properties\": {\n        \"address\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"maxLength\": 160\n        },\n        \"senderAddress\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/wireless-apis-send-sms-request-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Send SMS Request
---
