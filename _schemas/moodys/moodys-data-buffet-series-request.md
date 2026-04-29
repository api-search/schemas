---
description: A single series request within a multi-series call.
layout: schema
name: SeriesRequest
properties_list:
- description: The unique series mnemonic identifier.
  name: mnemonic
  type: string
- description: Desired output frequency.
  name: freq
  type: string
- description: Mathematical transformation to apply.
  name: trans
  type: string
- description: Start date for the data range.
  name: startDate
  type: string
- description: End date for the data range.
  name: endDate
  type: string
- description: Vintage date for historical data revisions.
  name: vintage
  type: string
provider_name: Moody's
provider_slug: moodys
schema_file: json-schema/moodys-data-buffet-series-request-schema.json
slug: moodys-data-buffet-series-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SeriesRequest\",\n  \"type\": \"object\",\n  \"description\": \"A single series request within a multi-series call.\",\n  \"properties\": {\n    \"mnemonic\": {\n      \"type\": \"string\",\n      \"description\": \"The unique series mnemonic identifier.\"\n    },\n    \"freq\": {\n      \"type\": \"string\",\n      \"description\": \"Desired output frequency.\"\n    },\n    \"trans\": {\n      \"type\": \"string\",\n      \"description\": \"Mathematical transformation to apply.\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"Start date for the data range.\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"End date for the data range.\"\n    },\n    \"vintage\": {\n      \"type\": \"string\",\n      \"description\": \"Vintage date for historical data revisions.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/json-schema/moodys-data-buffet-series-request-schema.json
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
title: SeriesRequest
---
