---
description: Defines a query specification for retrieving and aggregating data in Honeycomb. Queries are used across boards, triggers, SLOs, and query annotations.
layout: schema
name: Honeycomb Query Specification
properties_list:
- description: The calculations (aggregations) to perform on the query data.
  name: calculations
  type: array
- description: Filters to apply to events before aggregation.
  name: filters
  type: array
- description: How to combine multiple filters. Defaults to AND.
  name: filter_combination
  type: string
- description: Column names to group results by.
  name: breakdowns
  type: array
- description: Ordering rules for the query results.
  name: orders
  type: array
- description: Post-aggregation filters applied to calculated results.
  name: havings
  type: array
- description: The relative time range in seconds to query over.
  name: time_range
  type: integer
- description: Unix timestamp for the absolute query start time.
  name: start_time
  type: integer
- description: Unix timestamp for the absolute query end time.
  name: end_time
  type: integer
- description: The time granularity of results in seconds.
  name: granularity
  type: integer
- description: Maximum number of result rows to return.
  name: limit
  type: integer
provider_name: honeycomb
provider_slug: honeycomb
schema_file: json-schema/honeycomb-query-schema.json
slug: honeycomb-query
source_filename: honeycomb-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://honeycomb.io/schemas/honeycomb/query.json\",\n  \"title\": \"Honeycomb Query Specification\",\n  \"description\": \"Defines a query specification for retrieving and aggregating data in Honeycomb. Queries are used across boards, triggers, SLOs, and query annotations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"calculations\": {\n      \"type\": \"array\",\n      \"description\": \"The calculations (aggregations) to perform on the query data.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Calculation\"\n      }\n    },\n    \"filters\": {\n      \"type\": \"array\",\n      \"description\": \"Filters to apply to events before aggregation.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Filter\"\n      }\n    },\n    \"filter_combination\": {\n      \"type\": \"string\",\n      \"description\": \"How to combine multiple filters. Defaults to AND.\",\n      \"enum\": [\"\
  AND\", \"OR\"]\n    },\n    \"breakdowns\": {\n      \"type\": \"array\",\n      \"description\": \"Column names to group results by.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"orders\": {\n      \"type\": \"array\",\n      \"description\": \"Ordering rules for the query results.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Order\"\n      }\n    },\n    \"havings\": {\n      \"type\": \"array\",\n      \"description\": \"Post-aggregation filters applied to calculated results.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Having\"\n      }\n    },\n    \"time_range\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"The relative time range in seconds to query over.\"\n    },\n    \"start_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp for the absolute query start time.\"\n    },\n    \"end_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp for the\
  \ absolute query end time.\"\n    },\n    \"granularity\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"The time granularity of results in seconds.\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 1000,\n      \"description\": \"Maximum number of result rows to return.\"\n    }\n  },\n  \"$defs\": {\n    \"Calculation\": {\n      \"type\": \"object\",\n      \"description\": \"An aggregation calculation to perform.\",\n      \"required\": [\"op\"],\n      \"properties\": {\n        \"op\": {\n          \"type\": \"string\",\n          \"description\": \"The aggregation operation to perform.\",\n          \"enum\": [\n            \"COUNT\",\n            \"SUM\",\n            \"AVG\",\n            \"COUNT_DISTINCT\",\n            \"MAX\",\n            \"MIN\",\n            \"P001\",\n            \"P01\",\n            \"P05\",\n            \"P10\",\n            \"P25\",\n            \"P50\",\n        \
  \    \"P75\",\n            \"P90\",\n            \"P95\",\n            \"P99\",\n            \"P999\",\n            \"HEATMAP\",\n            \"RATE_AVG\",\n            \"RATE_SUM\",\n            \"RATE_MAX\"\n          ]\n        },\n        \"column\": {\n          \"type\": \"string\",\n          \"description\": \"The column to perform the calculation on. Not required for COUNT.\"\n        }\n      }\n    },\n    \"Filter\": {\n      \"type\": \"object\",\n      \"description\": \"A filter condition applied to events.\",\n      \"required\": [\"column\", \"op\"],\n      \"properties\": {\n        \"column\": {\n          \"type\": \"string\",\n          \"description\": \"The column name to filter on.\"\n        },\n        \"op\": {\n          \"type\": \"string\",\n          \"description\": \"The comparison operator.\",\n          \"enum\": [\n            \"=\",\n            \"!=\",\n            \">\",\n            \">=\",\n            \"<\",\n            \"<=\",\n            \"\
  starts-with\",\n            \"does-not-start-with\",\n            \"contains\",\n            \"does-not-contain\",\n            \"exists\",\n            \"does-not-exist\",\n            \"in\",\n            \"not-in\"\n          ]\n        },\n        \"value\": {\n          \"description\": \"The value to compare against. Not required for exists/does-not-exist operators.\"\n        }\n      }\n    },\n    \"Order\": {\n      \"type\": \"object\",\n      \"description\": \"An ordering rule for query results.\",\n      \"properties\": {\n        \"column\": {\n          \"type\": \"string\",\n          \"description\": \"The column to order by.\"\n        },\n        \"op\": {\n          \"type\": \"string\",\n          \"description\": \"The aggregation operation to order by, if ordering by a calculation.\"\n        },\n        \"order\": {\n          \"type\": \"string\",\n          \"description\": \"The sort direction.\",\n          \"enum\": [\"ascending\", \"descending\"]\n      \
  \  }\n      }\n    },\n    \"Having\": {\n      \"type\": \"object\",\n      \"description\": \"A post-aggregation filter applied to calculated results.\",\n      \"properties\": {\n        \"calculate_op\": {\n          \"type\": \"string\",\n          \"description\": \"The calculation operation this having clause applies to.\"\n        },\n        \"column\": {\n          \"type\": \"string\",\n          \"description\": \"The column the calculation is performed on.\"\n        },\n        \"op\": {\n          \"type\": \"string\",\n          \"description\": \"The comparison operator.\",\n          \"enum\": [\">\", \">=\", \"<\", \"<=\", \"=\", \"!=\"]\n        },\n        \"value\": {\n          \"type\": \"number\",\n          \"description\": \"The value to compare the calculated result against.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/json-schema/honeycomb-query-schema.json
tags: []
title: Honeycomb Query Specification
---
