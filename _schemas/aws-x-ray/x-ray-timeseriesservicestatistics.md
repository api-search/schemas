---
description: ''
layout: schema
name: TimeSeriesServiceStatistics
properties_list:
- description: ''
  name: Timestamp
  type: string
- description: ''
  name: EdgeSummaryStatistics
  type: object
- description: ''
  name: ServiceSummaryStatistics
  type: object
- description: ''
  name: ServiceForecastStatistics
  type: object
- description: ''
  name: ResponseTimeHistogram
  type: array
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-timeseriesservicestatistics-schema.json
slug: x-ray-timeseriesservicestatistics
source_filename: x-ray-timeseriesservicestatistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TimeSeriesServiceStatistics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"EdgeSummaryStatistics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"OkCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"ErrorStatistics\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"ThrottleCount\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            },\n            \"OtherCount\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            },\n            \"TotalCount\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            }\n          }\n        },\n        \"FaultStatistics\": {\n          \"type\": \"object\"\
  ,\n          \"properties\": {\n            \"OtherCount\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            },\n            \"TotalCount\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            }\n          }\n        },\n        \"TotalCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"TotalResponseTime\": {\n          \"type\": \"number\"\n        }\n      }\n    },\n    \"ServiceSummaryStatistics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"OkCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"ErrorStatistics\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"ThrottleCount\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            },\n            \"OtherCount\": {\n              \"type\": \"integer\",\n              \"format\"\
  : \"int64\"\n            },\n            \"TotalCount\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            }\n          }\n        },\n        \"FaultStatistics\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"OtherCount\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            },\n            \"TotalCount\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            }\n          }\n        },\n        \"TotalCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"TotalResponseTime\": {\n          \"type\": \"number\"\n        }\n      }\n    },\n    \"ServiceForecastStatistics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"FaultCountHigh\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"FaultCountLow\": {\n          \"type\": \"integer\"\
  ,\n          \"format\": \"int64\"\n        }\n      }\n    },\n    \"ResponseTimeHistogram\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Value\": {\n            \"type\": \"number\"\n          },\n          \"Count\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-timeseriesservicestatistics-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: TimeSeriesServiceStatistics
---
