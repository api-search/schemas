---
description: A metadata label applied to an Amazon Forecast resource.
layout: schema
name: Tag
properties_list:
- description: Tag key.
  name: Key
  type: string
- description: Tag value.
  name: Value
  type: string
provider_name: Amazon Forecast
provider_slug: amazon-forecast
schema_file: json-schema/amazon-forecast-tag-schema.json
slug: amazon-forecast-tag
source_filename: amazon-forecast-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-forecast/refs/heads/main/json-schema/amazon-forecast-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A metadata label applied to an Amazon Forecast resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"Tag key.\"\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"Tag value.\"\n    }\n  },\n  \"required\": [\n    \"Key\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-forecast/refs/heads/main/json-schema/amazon-forecast-tag-schema.json
tags:
- Forecasting
- Machine Learning
- Predictive Analytics
- Time Series
title: Tag
---
