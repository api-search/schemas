---
description: Verification schema from Bandwidth toll-free-verification API
layout: schema
name: Verification
properties_list:
- description: The unique identifier for the verification request
  name: verificationId
  type: string
- description: The toll-free numbers associated with this verification
  name: telephoneNumbers
  type: array
- description: The current verification status
  name: status
  type: string
- description: The business name on the verification
  name: businessName
  type: string
- description: The messaging use case
  name: useCase
  type: string
- description: The date and time the verification was submitted
  name: submissionDate
  type: string
- description: The date and time the verification was approved or denied
  name: verificationDate
  type: string
- description: The reason for denial, if the verification was denied
  name: denialReason
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/toll-free-verification-verification-schema.json
slug: toll-free-verification-verification
source_filename: toll-free-verification-verification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/toll-free-verification-verification-schema.json\",\n  \"title\": \"Verification\",\n  \"description\": \"Verification schema from Bandwidth toll-free-verification API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"verificationId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the verification request\"\n    },\n    \"telephoneNumbers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The toll-free numbers associated with this verification\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING_VERIFICATION\",\n        \"VERIFIED\",\n        \"RESTRICTED\",\n        \"DENIED\",\n        \"SUBMITTED\"\n      ],\n      \"description\": \"The current verification\
  \ status\"\n    },\n    \"businessName\": {\n      \"type\": \"string\",\n      \"description\": \"The business name on the verification\"\n    },\n    \"useCase\": {\n      \"type\": \"string\",\n      \"description\": \"The messaging use case\"\n    },\n    \"submissionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the verification was submitted\"\n    },\n    \"verificationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the verification was approved or denied\"\n    },\n    \"denialReason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason for denial, if the verification was denied\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/toll-free-verification-verification-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Verification
---
