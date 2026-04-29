---
description: Response after sending SMS via AT&T Wireless APIs
layout: schema
name: Send SMS Response
properties_list:
- description: ''
  name: outboundSMSResponse
  type: object
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/wireless-apis-send-sms-response-schema.json
slug: wireless-apis-send-sms-response
source_filename: wireless-apis-send-sms-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.att.com/schemas/wireless/send-sms-response\",\n  \"title\": \"Send SMS Response\",\n  \"description\": \"Response after sending SMS via AT&T Wireless APIs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"outboundSMSResponse\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"messageId\": {\n          \"type\": \"string\"\n        },\n        \"resourceReference\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"resourceURL\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/wireless-apis-send-sms-response-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Send SMS Response
---
