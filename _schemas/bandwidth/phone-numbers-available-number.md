---
description: An available phone number from Bandwidth inventory
layout: schema
name: AvailableNumber
properties_list:
- description: The full phone number in E.164 format
  name: fullNumber
  type: string
- description: The city associated with the number
  name: city
  type: string
- description: The state associated with the number
  name: state
  type: string
- description: The LATA code for the number
  name: lata
  type: string
- description: The rate center for the number
  name: rateCenter
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-available-number-schema.json
slug: phone-numbers-available-number
source_filename: phone-numbers-available-number-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-available-number-schema.json\",\n  \"title\": \"AvailableNumber\",\n  \"description\": \"An available phone number from Bandwidth inventory\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fullNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The full phone number in E.164 format\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city associated with the number\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state associated with the number\"\n    },\n    \"lata\": {\n      \"type\": \"string\",\n      \"description\": \"The LATA code for the number\"\n    },\n    \"rateCenter\": {\n      \"type\": \"string\",\n      \"description\": \"The rate center for the number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-available-number-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: AvailableNumber
---
