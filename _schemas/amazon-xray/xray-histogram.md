---
description: Histogram schema from Amazon X-Ray API
layout: schema
name: Histogram
properties_list: []
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-histogram-schema.json
slug: xray-histogram
source_filename: xray-histogram-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/HistogramEntry\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Histogram\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-histogram-schema.json\",\n  \"description\": \"Histogram schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-histogram-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: Histogram
---
