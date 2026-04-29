---
description: ''
layout: schema
name: HistogramEntry
properties_list:
- description: ''
  name: Value
  type: number
- description: ''
  name: Count
  type: integer
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-histogramentry-schema.json
slug: x-ray-histogramentry
source_filename: x-ray-histogramentry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HistogramEntry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Value\": {\n      \"type\": \"number\"\n    },\n    \"Count\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-histogramentry-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: HistogramEntry
---
