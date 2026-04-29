---
description: Request body for retrieving multiple series simultaneously.
layout: schema
name: MultiSeriesRequest
properties_list:
- description: Array of series requests. Maximum 25 series per request.
  name: series
  type: array
provider_name: Moody's
provider_slug: moodys
schema_file: json-schema/moodys-data-buffet-multi-series-request-schema.json
slug: moodys-data-buffet-multi-series-request
source_filename: moodys-data-buffet-multi-series-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MultiSeriesRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for retrieving multiple series simultaneously.\",\n  \"properties\": {\n    \"series\": {\n      \"type\": \"array\",\n      \"description\": \"Array of series requests. Maximum 25 series per request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/json-schema/moodys-data-buffet-multi-series-request-schema.json
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
title: MultiSeriesRequest
---
