---
description: Response containing a list of available phone numbers
layout: schema
name: AvailableNumbersResponse
properties_list:
- description: The number of results returned
  name: resultCount
  type: integer
- description: ''
  name: telephoneNumberList
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-available-numbers-response-schema.json
slug: phone-numbers-available-numbers-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-available-numbers-response-schema.json\",\n  \"title\": \"AvailableNumbersResponse\",\n  \"description\": \"Response containing a list of available phone numbers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resultCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of results returned\"\n    },\n    \"telephoneNumberList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AvailableNumber\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-available-numbers-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: AvailableNumbersResponse
---
