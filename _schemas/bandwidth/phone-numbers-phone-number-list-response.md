---
description: Response containing a list of phone numbers
layout: schema
name: PhoneNumberListResponse
properties_list:
- description: Total number of phone numbers
  name: totalCount
  type: integer
- description: ''
  name: telephoneNumbers
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-phone-number-list-response-schema.json
slug: phone-numbers-phone-number-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-phone-number-list-response-schema.json\",\n  \"title\": \"PhoneNumberListResponse\",\n  \"description\": \"Response containing a list of phone numbers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of phone numbers\"\n    },\n    \"telephoneNumbers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PhoneNumber\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-phone-number-list-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: PhoneNumberListResponse
---
