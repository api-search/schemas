---
description: JSON Schema for a single FRED data observation (data point) in an economic time series.
layout: schema
name: FRED Economic Data Observation
properties_list:
- description: Realtime start date for this observation.
  name: realtime_start
  type: string
- description: Realtime end date for this observation.
  name: realtime_end
  type: string
- description: The observation date.
  name: date
  type: string
- description: The observation value. A period (.) indicates a missing value.
  name: value
  type: string
provider_name: Reserve Requirements
provider_slug: reserve-requirements
schema_file: json-schema/fred-observation-schema.json
slug: fred-observation
source_filename: fred-observation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/reserve-requirements/json-schema/fred-observation-schema.json\",\n  \"title\": \"FRED Economic Data Observation\",\n  \"description\": \"JSON Schema for a single FRED data observation (data point) in an economic time series.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"realtime_start\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Realtime start date for this observation.\"\n    },\n    \"realtime_end\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Realtime end date for this observation.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The observation date.\",\n      \"example\": \"2024-01-03\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The observation value. A period (.)\
  \ indicates a missing value.\",\n      \"example\": \"3459214\"\n    }\n  },\n  \"required\": [\"date\", \"value\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reserve-requirements/refs/heads/main/json-schema/fred-observation-schema.json
tags:
- Reserve Requirements
- Federal Reserve
- Banking Regulation
- Monetary Policy
- Regulation D
- Finance
title: FRED Economic Data Observation
---
