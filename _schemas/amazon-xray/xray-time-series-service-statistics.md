---
description: A list of TimeSeriesStatistic structures.
layout: schema
name: TimeSeriesServiceStatistics
properties_list:
- description: ''
  name: Timestamp
  type: object
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
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-time-series-service-statistics-schema.json
slug: xray-time-series-service-statistics
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Timestamp of the window for which statistics are aggregated.\"\n        }\n      ]\n    },\n    \"EdgeSummaryStatistics\": {\n      \"$ref\": \"#/components/schemas/EdgeStatistics\"\n    },\n    \"ServiceSummaryStatistics\": {\n      \"$ref\": \"#/components/schemas/ServiceStatistics\"\n    },\n    \"ServiceForecastStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ForecastStatistics\"\n        },\n        {\n          \"description\": \"The forecasted high and low fault count values.\"\n        }\n      ]\n    },\n    \"ResponseTimeHistogram\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Histogram\"\n        },\n        {\n          \"description\": \"The response time histogram for the selected\
  \ entities.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A list of TimeSeriesStatistic structures.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TimeSeriesServiceStatistics\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-time-series-service-statistics-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-time-series-service-statistics-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: TimeSeriesServiceStatistics
---
