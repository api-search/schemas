---
description: ''
layout: schema
name: InsightSummary
properties_list:
- description: ''
  name: InsightId
  type: string
- description: ''
  name: GroupARN
  type: string
- description: ''
  name: GroupName
  type: string
- description: ''
  name: RootCauseServiceId
  type: object
- description: ''
  name: Categories
  type: array
- description: ''
  name: State
  type: string
- description: ''
  name: StartTime
  type: string
- description: ''
  name: EndTime
  type: string
- description: ''
  name: Summary
  type: string
- description: ''
  name: ClientRequestImpactStatistics
  type: object
- description: ''
  name: RootCauseServiceRequestImpactStatistics
  type: object
- description: ''
  name: TopAnomalousServices
  type: array
- description: ''
  name: LastUpdateTime
  type: string
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-insightsummary-schema.json
slug: x-ray-insightsummary
source_filename: x-ray-insightsummary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InsightSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InsightId\": {\n      \"type\": \"string\"\n    },\n    \"GroupARN\": {\n      \"type\": \"string\"\n    },\n    \"GroupName\": {\n      \"type\": \"string\"\n    },\n    \"RootCauseServiceId\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Name\": {\n          \"type\": \"string\"\n        },\n        \"Names\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"AccountId\": {\n          \"type\": \"string\"\n        },\n        \"Type\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"FAULT\"\n        ]\n      }\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"\
  enum\": [\n        \"ACTIVE\",\n        \"CLOSED\"\n      ]\n    },\n    \"StartTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"EndTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"Summary\": {\n      \"type\": \"string\"\n    },\n    \"ClientRequestImpactStatistics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"FaultCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"OkCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"TotalCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        }\n      }\n    },\n    \"RootCauseServiceRequestImpactStatistics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"FaultCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"OkCount\": {\n          \"type\": \"integer\"\
  ,\n          \"format\": \"int64\"\n        },\n        \"TotalCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        }\n      }\n    },\n    \"TopAnomalousServices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"ServiceId\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Name\": {\n                \"type\": \"string\"\n              },\n              \"Names\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"AccountId\": {\n                \"type\": \"string\"\n              },\n              \"Type\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"LastUpdateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-insightsummary-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: InsightSummary
---
