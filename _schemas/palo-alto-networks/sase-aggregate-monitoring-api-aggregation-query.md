---
description: AggregationQuery schema from Palo Alto Networks SASE Aggregate Monitoring API
layout: schema
name: AggregationQuery
properties_list:
- description: Tenant Service Group ID to scope the query. Data from all descendant TSGs within this scope is included.
  name: tsg_id
  type: string
- description: Key-value filter conditions to apply to the query. Filter keys are data-type specific (e.g., severity, category, app_name).
  name: filter
  type: object
- description: Time range for the query.
  name: time_range
  type: object
- description: Maximum number of result rows to return.
  name: count
  type: integer
- description: Configuration for time-series histogram output. When specified, results are bucketed by time.
  name: histogram
  type: object
- description: Dimension fields to group results by. Supported values are data-type specific.
  name: group_by
  type: array
- description: Sort order for results.
  name: sort
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-aggregate-monitoring-api-aggregation-query-schema.json
slug: sase-aggregate-monitoring-api-aggregation-query
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AggregationQuery\",\n  \"description\": \"AggregationQuery schema from Palo Alto Networks SASE Aggregate Monitoring API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-aggregate-monitoring-api-aggregation-query-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tsg_id\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant Service Group ID to scope the query. Data from all descendant TSGs within this scope is included.\"\n    },\n    \"filter\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value filter conditions to apply to the query. Filter keys are data-type specific (e.g., severity, category, app_name).\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"time_range\": {\n      \"type\": \"object\",\n      \"description\": \"Time range for\
  \ the query.\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Query start time (ISO 8601).\"\n        },\n        \"end\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Query end time (ISO 8601). Defaults to current time.\"\n        },\n        \"last\": {\n          \"type\": \"string\",\n          \"description\": \"Relative time range shorthand (e.g., 1h, 24h, 7d, 30d). Mutually exclusive with start/end.\"\n        }\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of result rows to return.\",\n      \"default\": 100,\n      \"maximum\": 1000\n    },\n    \"histogram\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for time-series histogram output. When specified, results are bucketed by time.\",\n      \"properties\": {\n        \"field\": {\n \
  \         \"type\": \"string\",\n          \"description\": \"Timestamp field to use for bucketing.\"\n        },\n        \"interval\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"1m\",\n            \"5m\",\n            \"15m\",\n            \"1h\",\n            \"6h\",\n            \"1d\"\n          ],\n          \"description\": \"Time bucket interval.\"\n        }\n      }\n    },\n    \"group_by\": {\n      \"type\": \"array\",\n      \"description\": \"Dimension fields to group results by. Supported values are data-type specific.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"sort\": {\n      \"type\": \"array\",\n      \"description\": \"Sort order for results.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"field\": {\n            \"type\": \"string\",\n            \"description\": \"Field name to sort by.\"\n          },\n          \"order\": {\n            \"type\": \"string\"\
  ,\n            \"enum\": [\n              \"asc\",\n              \"desc\"\n            ],\n            \"default\": \"desc\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"tsg_id\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-aggregate-monitoring-api-aggregation-query-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AggregationQuery
---
