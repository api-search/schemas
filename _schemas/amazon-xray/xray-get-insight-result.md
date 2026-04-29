---
description: GetInsightResult schema from Amazon X-Ray API
layout: schema
name: GetInsightResult
properties_list:
- description: ''
  name: Insight
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-insight-result-schema.json
slug: xray-get-insight-result
source_filename: xray-get-insight-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Insight\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Insight\"\n        },\n        {\n          \"description\": \"The summary information of an insight.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetInsightResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-insight-result-schema.json\",\n  \"description\": \"GetInsightResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-insight-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetInsightResult
---
