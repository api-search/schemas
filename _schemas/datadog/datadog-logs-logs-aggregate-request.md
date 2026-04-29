---
description: Request body for aggregating log events
layout: schema
name: LogsAggregateRequest
properties_list:
- description: ''
  name: filter
  type: object
- description: List of aggregation computations to perform on the filtered log set
  name: compute
  type: array
- description: List of facets to group results by, enabling breakdown by log attribute
  name: group_by
  type: array
- description: Options for the aggregation query
  name: options
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-logs-logs-aggregate-request-schema.json
slug: datadog-logs-logs-aggregate-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-logs-aggregate-request-schema.json\",\n  \"title\": \"LogsAggregateRequest\",\n  \"description\": \"Request body for aggregating log events\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filter\": {\n      \"$ref\": \"#/components/schemas/LogsQueryFilter\"\n    },\n    \"compute\": {\n      \"type\": \"array\",\n      \"description\": \"List of aggregation computations to perform on the filtered log set\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LogsCompute\"\n      }\n    },\n    \"group_by\": {\n      \"type\": \"array\",\n      \"description\": \"List of facets to group results by, enabling breakdown by log attribute\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LogsGroupBy\"\n      }\n    },\n    \"options\": {\n      \"type\": \"object\",\n  \
  \    \"description\": \"Options for the aggregation query\",\n      \"properties\": {\n        \"timezone\": {\n          \"type\": \"string\",\n          \"description\": \"The timezone to use for time-based group-by operations (IANA timezone name)\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-logs-aggregate-request-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: LogsAggregateRequest
---
