---
description: AuthenticationResultResponse schema from Adyen API
layout: schema
name: AuthenticationResultResponse
properties_list:
- description: The result of the 3D Secure authentication.
  name: threeDS1Result
  type: object
- description: The result of the 3D Secure 2 authentication.
  name: threeDS2Result
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-authentication-result-response-schema.json
slug: payments-authentication-result-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-authentication-result-response-schema.json\",\n  \"title\": \"AuthenticationResultResponse\",\n  \"description\": \"AuthenticationResultResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"threeDS1Result\": {\n      \"description\": \"The result of the 3D Secure authentication.\",\n      \"$ref\": \"#/components/schemas/ThreeDS1Result\"\n    },\n    \"threeDS2Result\": {\n      \"description\": \"The result of the 3D Secure 2 authentication.\",\n      \"$ref\": \"#/components/schemas/ThreeDS2Result\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-authentication-result-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AuthenticationResultResponse
---
