---
description: VerificationListResponse schema from Bandwidth toll-free-verification API
layout: schema
name: VerificationListResponse
properties_list:
- description: Total number of verification requests
  name: totalCount
  type: integer
- description: ''
  name: verifications
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/toll-free-verification-verification-list-response-schema.json
slug: toll-free-verification-verification-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/toll-free-verification-verification-list-response-schema.json\",\n  \"title\": \"VerificationListResponse\",\n  \"description\": \"VerificationListResponse schema from Bandwidth toll-free-verification API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of verification requests\"\n    },\n    \"verifications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Verification\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/toll-free-verification-verification-list-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: VerificationListResponse
---
