---
description: The date parameters for Publisher calculation.
layout: schema
name: PubDateParameters
properties_list:
- description: Calculation's start date.
  name: startdate
  type: string
- description: Calculation's end date or as of date.
  name: enddate
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-publisher-pub-date-parameters-schema.json
slug: factset-publisher-pub-date-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PubDateParameters\",\n  \"type\": \"object\",\n  \"description\": \"The date parameters for Publisher calculation.\",\n  \"properties\": {\n    \"startdate\": {\n      \"type\": \"string\",\n      \"description\": \"Calculation's start date.\"\n    },\n    \"enddate\": {\n      \"type\": \"string\",\n      \"description\": \"Calculation's end date or as of date.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-publisher-pub-date-parameters-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: PubDateParameters
---
