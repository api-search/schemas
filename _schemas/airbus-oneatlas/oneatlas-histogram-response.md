---
description: ''
layout: schema
name: HistogramResponse
properties_list:
- description: ''
  name: histograms
  type: array
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-histogram-response-schema.json
slug: oneatlas-histogram-response
source_filename: oneatlas-histogram-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-histogram-response-schema.json\",\n  \"title\": \"HistogramResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"histograms\": {\n      \"items\": {\n        \"properties\": {\n          \"band\": {\n            \"example\": \"B0\",\n            \"type\": \"string\"\n          },\n          \"max\": {\n            \"example\": 9613,\n            \"format\": \"integer\",\n            \"minimum\": 1,\n            \"type\": \"number\"\n          },\n          \"mean\": {\n            \"example\": 785.7152806485769,\n            \"format\": \"float\",\n            \"minimum\": 1,\n            \"type\": \"number\"\n          },\n          \"min\": {\n            \"example\": 1,\n            \"format\": \"integer\",\n            \"minimum\": 1,\n            \"type\": \"number\"\n        \
  \  },\n          \"stdev\": {\n            \"example\": 364.8379459959255,\n            \"format\": \"float\",\n            \"minimum\": 1,\n            \"type\": \"number\"\n          },\n          \"step\": {\n            \"example\": 1,\n            \"format\": \"integer\",\n            \"minimum\": 1,\n            \"type\": \"number\"\n          },\n          \"values\": {\n            \"example\": [\n              3,\n              0,\n              0,\n              6\n            ],\n            \"items\": {\n              \"format\": \"integer\",\n              \"minimum\": 0,\n              \"type\": \"number\"\n            },\n            \"minItems\": 1,\n            \"type\": \"array\"\n          }\n        },\n        \"type\": \"object\"\n      },\n      \"minItems\": 1,\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-histogram-response-schema.json
tags:
- Imagery
- Satellites
title: HistogramResponse
---
