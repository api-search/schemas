---
description: NumberVerificationResponse schema
layout: schema
name: NumberVerificationResponse
properties_list:
- description: True if the device's network connection matches the provided phone number, false otherwise.
  name: devicePhoneNumberVerified
  type: boolean
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/number-verification-api-number-verification-response-schema.json
slug: number-verification-api-number-verification-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/number-verification-api-number-verification-response-schema.json\",\n  \"title\": \"NumberVerificationResponse\",\n  \"description\": \"NumberVerificationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"devicePhoneNumberVerified\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the device's network connection matches the provided phone number, false otherwise.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/number-verification-api-number-verification-response-schema.json
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: NumberVerificationResponse
---
