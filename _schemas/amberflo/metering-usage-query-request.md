---
description: Request body for querying usage data
layout: schema
name: UsageQueryRequest
properties_list:
- description: Name of the meter to query
  name: meterApiName
  type: string
- description: Query start time in Unix seconds
  name: startTimeInSeconds
  type: integer
- description: Query end time in Unix seconds
  name: endTimeInSeconds
  type: integer
- description: Aggregation function to apply
  name: aggregation
  type: string
- description: Time interval for grouping results
  name: timeGroupingInterval
  type: string
- description: Dimensions to group results by
  name: groupBy
  type: array
- description: List of customer IDs to filter by
  name: customerFilter
  type: array
- description: Key-value filter for dimension-based filtering
  name: filter
  type: object
provider_name: Amberflo
provider_slug: amberflo
schema_file: json-schema/metering-usage-query-request-schema.json
slug: metering-usage-query-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/metering-usage-query-request-schema.json\",\n  \"title\": \"UsageQueryRequest\",\n  \"description\": \"Request body for querying usage data\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meterApiName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the meter to query\",\n      \"example\": \"api-calls\"\n    },\n    \"startTimeInSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Query start time in Unix seconds\",\n      \"example\": 1718100000\n    },\n    \"endTimeInSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Query end time in Unix seconds\",\n      \"example\": 1718186400\n    },\n    \"aggregation\": {\n      \"type\": \"string\",\n      \"description\": \"Aggregation function to apply\",\n      \"enum\": [\n        \"SUM\",\n        \"\
  MAX\",\n        \"COUNT\"\n      ],\n      \"example\": \"SUM\"\n    },\n    \"timeGroupingInterval\": {\n      \"type\": \"string\",\n      \"description\": \"Time interval for grouping results\",\n      \"enum\": [\n        \"HOUR\",\n        \"DAY\",\n        \"WEEK\",\n        \"MONTH\"\n      ],\n      \"example\": \"DAY\"\n    },\n    \"groupBy\": {\n      \"type\": \"array\",\n      \"description\": \"Dimensions to group results by\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"customerId\"\n      ]\n    },\n    \"customerFilter\": {\n      \"type\": \"array\",\n      \"description\": \"List of customer IDs to filter by\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"filter\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      },\n      \"description\": \"Key-value filter for dimension-based\
  \ filtering\"\n    }\n  },\n  \"required\": [\n    \"meterApiName\",\n    \"startTimeInSeconds\",\n    \"endTimeInSeconds\",\n    \"aggregation\",\n    \"timeGroupingInterval\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/metering-usage-query-request-schema.json
tags:
- Usage-Based Billing
- Metering
- FinOps
- AI Cost Management
- Billing
- Monetization
title: UsageQueryRequest
---
