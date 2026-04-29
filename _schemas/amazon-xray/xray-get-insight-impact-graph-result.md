---
description: GetInsightImpactGraphResult schema from Amazon X-Ray API
layout: schema
name: GetInsightImpactGraphResult
properties_list:
- description: ''
  name: InsightId
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: ServiceGraphStartTime
  type: object
- description: ''
  name: ServiceGraphEndTime
  type: object
- description: ''
  name: Services
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-insight-impact-graph-result-schema.json
slug: xray-get-insight-impact-graph-result
source_filename: xray-get-insight-impact-graph-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"InsightId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightId\"\n        },\n        {\n          \"description\": \"The insight's unique identifier.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The provided start time.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The provided end time. \"\n        }\n      ]\n    },\n    \"ServiceGraphStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time, in Unix seconds, at which the service graph started.\"\n        }\n      ]\n    },\n    \"ServiceGraphEndTime\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time, in Unix seconds, at which the service graph ended.\"\n        }\n      ]\n    },\n    \"Services\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightImpactGraphServiceList\"\n        },\n        {\n          \"description\": \"The Amazon Web Services instrumented services related to the insight.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetInsightImpactGraphResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-insight-impact-graph-result-schema.json\",\n  \"\
  description\": \"GetInsightImpactGraphResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-insight-impact-graph-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetInsightImpactGraphResult
---
