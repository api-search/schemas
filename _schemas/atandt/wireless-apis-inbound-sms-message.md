---
description: Inbound SMS message received via AT&T
layout: schema
name: Inbound SMS Message
properties_list:
- description: ''
  name: messageId
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: senderAddress
  type: string
- description: ''
  name: destinationAddress
  type: string
- description: ''
  name: dateTime
  type: string
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/wireless-apis-inbound-sms-message-schema.json
slug: wireless-apis-inbound-sms-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.att.com/schemas/wireless/inbound-sms-message\",\n  \"title\": \"Inbound SMS Message\",\n  \"description\": \"Inbound SMS message received via AT&T\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messageId\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"senderAddress\": {\n      \"type\": \"string\"\n    },\n    \"destinationAddress\": {\n      \"type\": \"string\"\n    },\n    \"dateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/wireless-apis-inbound-sms-message-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Inbound SMS Message
---
