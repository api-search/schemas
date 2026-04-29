---
description: VerificationResponse schema from AgeChecker.Net API
layout: schema
name: VerificationResponse
properties_list:
- description: Verification outcome.
  name: result
  type: string
- description: Unique session identifier for this verification.
  name: session_id
  type: string
- description: Whether the customer must upload a photo ID to complete verification.
  name: requires_photo_id
  type: boolean
- description: Whether age was successfully verified.
  name: age_verified
  type: boolean
- description: The minimum age threshold checked.
  name: minimum_age
  type: integer
- description: URL to redirect customer if photo ID is required.
  name: redirect_url
  type: string
provider_name: AgeChecker.Net
provider_slug: agechecker-net
schema_file: json-schema/age-verification-verification-response-schema.json
slug: age-verification-verification-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agechecker-net/refs/heads/main/json-schema/age-verification-verification-response-schema.json\",\n  \"title\": \"VerificationResponse\",\n  \"description\": \"VerificationResponse schema from AgeChecker.Net API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"result\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pass\",\n        \"fail\",\n        \"pending\"\n      ],\n      \"description\": \"Verification outcome.\",\n      \"example\": \"pass\"\n    },\n    \"session_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique session identifier for this verification.\",\n      \"example\": \"500123\"\n    },\n    \"requires_photo_id\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the customer must upload a photo ID to complete verification.\",\n      \"example\": true\n    },\n    \"age_verified\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether age was successfully verified.\",\n      \"example\": true\n    },\n    \"minimum_age\": {\n      \"type\": \"integer\",\n      \"description\": \"The minimum age threshold checked.\",\n      \"example\": 1\n    },\n    \"redirect_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to redirect customer if photo ID is required.\",\n      \"example\": \"https://example.com\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agechecker-net/refs/heads/main/json-schema/age-verification-verification-response-schema.json
tags:
- Age Verification
- Identity
- Compliance
- Regulatory
- E-Commerce
title: VerificationResponse
---
