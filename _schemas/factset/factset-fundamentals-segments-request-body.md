---
description: Request parameters for segment data.
layout: schema
name: SegmentsRequestBody
properties_list:
- description: Segment metric. SALES, OPINC, ASSETS, DEP, or CAPEX.
  name: metrics
  type: string
- description: Segment type. BUS = Business, GEO = Geographic.
  name: segmentType
  type: string
- description: Segment periodicity. ANN or ANN_R only.
  name: periodicity
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fundamentals-segments-request-body-schema.json
slug: factset-fundamentals-segments-request-body
source_filename: factset-fundamentals-segments-request-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SegmentsRequestBody\",\n  \"type\": \"object\",\n  \"description\": \"Request parameters for segment data.\",\n  \"properties\": {\n    \"metrics\": {\n      \"type\": \"string\",\n      \"description\": \"Segment metric. SALES, OPINC, ASSETS, DEP, or CAPEX.\"\n    },\n    \"segmentType\": {\n      \"type\": \"string\",\n      \"description\": \"Segment type. BUS = Business, GEO = Geographic.\"\n    },\n    \"periodicity\": {\n      \"type\": \"string\",\n      \"description\": \"Segment periodicity. ANN or ANN_R only.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fundamentals-segments-request-body-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: SegmentsRequestBody
---
