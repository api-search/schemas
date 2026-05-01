---
description: The name and value of a sampling rule to apply to a trace summary.
layout: schema
name: SamplingStrategy
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-sampling-strategy-schema.json
slug: xray-sampling-strategy
source_filename: xray-sampling-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamplingStrategyName\"\n        },\n        {\n          \"description\": \"The name of a sampling rule.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableDouble\"\n        },\n        {\n          \"description\": \"The value of a sampling rule.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The name and value of a sampling rule to apply to a trace summary.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SamplingStrategy\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-sampling-strategy-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-sampling-strategy-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: SamplingStrategy
---
