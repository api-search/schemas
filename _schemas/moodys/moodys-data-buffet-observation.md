---
description: A single time series observation or forecast data point.
layout: schema
name: Observation
properties_list:
- description: The observation date in YYYY-MM-DD format. For frequencies coarser than daily, represents the period start date.
  name: date
  type: string
- description: The observation value. Null indicates missing or unavailable data for this period.
  name: value
  type: '[''number'', ''null'']'
- description: Status indicator for the data point.
  name: status
  type: string
provider_name: Moody's
provider_slug: moodys
schema_file: json-schema/moodys-data-buffet-observation-schema.json
slug: moodys-data-buffet-observation
source_filename: moodys-data-buffet-observation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Observation\",\n  \"type\": \"object\",\n  \"description\": \"A single time series observation or forecast data point.\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"The observation date in YYYY-MM-DD format. For frequencies coarser than daily, represents the period start date.\"\n    },\n    \"value\": {\n      \"type\": \"['number', 'null']\",\n      \"description\": \"The observation value. Null indicates missing or unavailable data for this period.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status indicator for the data point.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/json-schema/moodys-data-buffet-observation-schema.json
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
title: Observation
---
