---
description: GetTimeSeriesServiceStatisticsRequest schema from Amazon X-Ray API
layout: schema
name: GetTimeSeriesServiceStatisticsRequest
properties_list:
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: GroupName
  type: object
- description: ''
  name: GroupARN
  type: object
- description: ''
  name: EntitySelectorExpression
  type: object
- description: ''
  name: Period
  type: object
- description: ''
  name: ForecastStatistics
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-time-series-service-statistics-request-schema.json
slug: xray-get-time-series-service-statistics-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"StartTime\",\n    \"EndTime\"\n  ],\n  \"title\": \"GetTimeSeriesServiceStatisticsRequest\",\n  \"properties\": {\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start of the time frame for which to aggregate statistics.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The end of the time frame for which to aggregate statistics.\"\n        }\n      ]\n    },\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupName\"\n        },\n        {\n          \"description\": \"The case-sensitive name of the group for which to pull statistics from.\"\n        }\n      ]\n    },\n    \"GroupARN\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/GroupARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the group for which to pull statistics from.\"\n        }\n      ]\n    },\n    \"EntitySelectorExpression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntitySelectorExpression\"\n        },\n        {\n          \"description\": \"A filter expression defining entities that will be aggregated for statistics. Supports ID, service, and edge functions. If no selector expression is specified, edge statistics are returned. \"\n        }\n      ]\n    },\n    \"Period\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"Aggregation period in seconds.\"\n        }\n      ]\n    },\n    \"ForecastStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n      \
  \  {\n          \"description\": \"The forecasted high and low fault count values. Forecast enabled requests require the EntitySelectorExpression ID be provided.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-time-series-service-statistics-request-schema.json\",\n  \"description\": \"GetTimeSeriesServiceStatisticsRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-time-series-service-statistics-request-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetTimeSeriesServiceStatisticsRequest
---
