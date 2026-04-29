---
description: Request to disconnect phone numbers
layout: schema
name: DisconnectRequest
properties_list:
- description: A name for the disconnect order
  name: name
  type: string
- description: ''
  name: disconnectTelephoneNumberOrderType
  type: object
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-disconnect-request-schema.json
slug: phone-numbers-disconnect-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-disconnect-request-schema.json\",\n  \"title\": \"DisconnectRequest\",\n  \"description\": \"Request to disconnect phone numbers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A name for the disconnect order\"\n    },\n    \"disconnectTelephoneNumberOrderType\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"telephoneNumberList\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"List of phone numbers to disconnect\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-disconnect-request-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: DisconnectRequest
---
