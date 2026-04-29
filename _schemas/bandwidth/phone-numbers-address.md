---
description: A physical address
layout: schema
name: Address
properties_list:
- description: The house/building number
  name: houseNumber
  type: string
- description: The street name
  name: streetName
  type: string
- description: The city
  name: city
  type: string
- description: The two-letter state code
  name: stateCode
  type: string
- description: The ZIP code
  name: zip
  type: string
- description: The country code
  name: country
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-address-schema.json
slug: phone-numbers-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"A physical address\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"houseNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The house/building number\"\n    },\n    \"streetName\": {\n      \"type\": \"string\",\n      \"description\": \"The street name\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city\"\n    },\n    \"stateCode\": {\n      \"type\": \"string\",\n      \"description\": \"The two-letter state code\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"The ZIP code\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The country code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-address-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Address
---
