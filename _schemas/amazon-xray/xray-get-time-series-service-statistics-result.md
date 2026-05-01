---
description: GetTimeSeriesServiceStatisticsResult schema from Amazon X-Ray API
layout: schema
name: GetTimeSeriesServiceStatisticsResult
properties_list:
- description: ''
  name: TimeSeriesServiceStatistics
  type: object
- description: ''
  name: ContainsOldGroupVersions
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-time-series-service-statistics-result-schema.json
slug: xray-get-time-series-service-statistics-result
source_filename: xray-get-time-series-service-statistics-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"TimeSeriesServiceStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeSeriesServiceStatisticsList\"\n        },\n        {\n          \"description\": \"The collection of statistics.\"\n        }\n      ]\n    },\n    \"ContainsOldGroupVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A flag indicating whether or not a group's filter expression has been consistent, or if a returned aggregation might show statistics from an older version of the group's filter expression.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"\
  title\": \"GetTimeSeriesServiceStatisticsResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-time-series-service-statistics-result-schema.json\",\n  \"description\": \"GetTimeSeriesServiceStatisticsResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-time-series-service-statistics-result-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetTimeSeriesServiceStatisticsResult
---
