---
description: Standard error response.
layout: schema
name: Error
properties_list:
- description: Machine-readable error code.
  name: code
  type: string
- description: Human-readable error message.
  name: message
  type: string
- description: Additional details about the error.
  name: details
  type: string
provider_name: Moody's
provider_slug: moodys
schema_file: json-schema/moodys-data-buffet-error-schema.json
slug: moodys-data-buffet-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable error code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message.\"\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"description\": \"Additional details about the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/json-schema/moodys-data-buffet-error-schema.json
tags:
- Climate Risk
- Compliance
- Credit Risk
- Economic Data
- Entity Verification
- Financial Analytics
- Insurance
- KYC
- Risk
- Screening
title: Error
---
