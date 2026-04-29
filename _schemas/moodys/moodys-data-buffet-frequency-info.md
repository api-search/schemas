---
description: Metadata about a supported data frequency.
layout: schema
name: FrequencyInfo
properties_list:
- description: Single-character frequency code used in API parameters.
  name: code
  type: string
- description: Human-readable frequency name.
  name: name
  type: string
- description: Description of the frequency and its typical use cases.
  name: description
  type: string
provider_name: Moody's
provider_slug: moodys
schema_file: json-schema/moodys-data-buffet-frequency-info-schema.json
slug: moodys-data-buffet-frequency-info
source_filename: moodys-data-buffet-frequency-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FrequencyInfo\",\n  \"type\": \"object\",\n  \"description\": \"Metadata about a supported data frequency.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Single-character frequency code used in API parameters.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable frequency name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the frequency and its typical use cases.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/json-schema/moodys-data-buffet-frequency-info-schema.json
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
title: FrequencyInfo
---
