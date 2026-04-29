---
description: A phone number assigned to the account
layout: schema
name: PhoneNumber
properties_list:
- description: The full phone number
  name: fullNumber
  type: string
- description: The city associated with the number
  name: city
  type: string
- description: The state associated with the number
  name: state
  type: string
- description: The LATA code
  name: lata
  type: string
- description: The rate center
  name: rateCenter
  type: string
- description: The current status of the number
  name: status
  type: string
- description: The site the number is assigned to
  name: siteId
  type: string
- description: The SIP peer the number is assigned to
  name: sipPeerId
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-phone-number-schema.json
slug: phone-numbers-phone-number
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-phone-number-schema.json\",\n  \"title\": \"PhoneNumber\",\n  \"description\": \"A phone number assigned to the account\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fullNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The full phone number\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city associated with the number\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state associated with the number\"\n    },\n    \"lata\": {\n      \"type\": \"string\",\n      \"description\": \"The LATA code\"\n    },\n    \"rateCenter\": {\n      \"type\": \"string\",\n      \"description\": \"The rate center\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status\
  \ of the number\"\n    },\n    \"siteId\": {\n      \"type\": \"string\",\n      \"description\": \"The site the number is assigned to\"\n    },\n    \"sipPeerId\": {\n      \"type\": \"string\",\n      \"description\": \"The SIP peer the number is assigned to\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-phone-number-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: PhoneNumber
---
