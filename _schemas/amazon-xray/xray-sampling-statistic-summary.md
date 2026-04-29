---
description: Aggregated request sampling data for a sampling rule across all services for a 10-second window.
layout: schema
name: SamplingStatisticSummary
properties_list:
- description: ''
  name: RuleName
  type: object
- description: ''
  name: Timestamp
  type: object
- description: ''
  name: RequestCount
  type: object
- description: ''
  name: BorrowCount
  type: object
- description: ''
  name: SampledCount
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-sampling-statistic-summary-schema.json
slug: xray-sampling-statistic-summary
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the sampling rule.\"\n        }\n      ]\n    },\n    \"Timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start time of the reporting window.\"\n        }\n      ]\n    },\n    \"RequestCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of requests that matched the rule.\"\n        }\n      ]\n    },\n    \"BorrowCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of requests recorded with borrowed reservoir quota.\"\n        }\n      ]\n \
  \   },\n    \"SampledCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of requests recorded.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Aggregated request sampling data for a sampling rule across all services for a 10-second window.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SamplingStatisticSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-sampling-statistic-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-sampling-statistic-summary-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: SamplingStatisticSummary
---
