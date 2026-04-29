---
description: Response containing multiple time series.
layout: schema
name: MultiSeriesResponse
properties_list:
- description: Array of time series responses.
  name: series
  type: array
provider_name: Moody's
provider_slug: moodys
schema_file: json-schema/moodys-data-buffet-multi-series-response-schema.json
slug: moodys-data-buffet-multi-series-response
source_filename: moodys-data-buffet-multi-series-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MultiSeriesResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response containing multiple time series.\",\n  \"properties\": {\n    \"series\": {\n      \"type\": \"array\",\n      \"description\": \"Array of time series responses.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/json-schema/moodys-data-buffet-multi-series-response-schema.json
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
title: MultiSeriesResponse
---
