---
description: Sampling statistics from a call to <a href="https://docs.aws.amazon.com/xray/latest/api/API_GetSamplingTargets.html">GetSamplingTargets</a> that X-Ray could not process.
layout: schema
name: UnprocessedStatistics
properties_list:
- description: ''
  name: RuleName
  type: object
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-unprocessed-statistics-schema.json
slug: xray-unprocessed-statistics
source_filename: xray-unprocessed-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the sampling rule.\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The error code.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The error message.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Sampling statistics from a call to <a href=\\\"https://docs.aws.amazon.com/xray/latest/api/API_GetSamplingTargets.html\\\">GetSamplingTargets</a> that X-Ray could not process.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UnprocessedStatistics\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-unprocessed-statistics-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-unprocessed-statistics-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: UnprocessedStatistics
---
