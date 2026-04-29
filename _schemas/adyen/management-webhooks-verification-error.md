---
description: VerificationError schema from Adyen API
layout: schema
name: VerificationError
properties_list:
- description: The verification error code.
  name: code
  type: string
- description: The verification error message.
  name: message
  type: string
- description: The actions that you can take to resolve the verification error.
  name: remediatingActions
  type: array
- description: More granular information about the verification error.
  name: subErrors
  type: array
- description: 'The type of verification error. Possible values: **invalidInput**, **dataMissing**, and **pendingStatus**.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-webhooks-verification-error-schema.json
slug: management-webhooks-verification-error
source_filename: management-webhooks-verification-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhooks-verification-error-schema.json\",\n  \"title\": \"VerificationError\",\n  \"description\": \"VerificationError schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"description\": \"The verification error code.\",\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"description\": \"The verification error message.\",\n      \"type\": \"string\"\n    },\n    \"remediatingActions\": {\n      \"description\": \"The actions that you can take to resolve the verification error.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RemediatingAction\"\n      },\n      \"type\": \"array\"\n    },\n    \"subErrors\": {\n      \"description\": \"More granular information about the verification error.\",\n      \"items\": {\n        \"$ref\"\
  : \"#/components/schemas/VerificationError-recursive\"\n      },\n      \"type\": \"array\"\n    },\n    \"type\": {\n      \"description\": \"The type of verification error.\\n\\nPossible values: **invalidInput**, **dataMissing**, and **pendingStatus**.\",\n      \"enum\": [\n        \"dataMissing\",\n        \"invalidInput\",\n        \"pendingStatus\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhooks-verification-error-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: VerificationError
---
