---
description: A cost query request used to analyze cloud spend using user-defined Finout Views, supporting date ranges and filters for granular cost insights.
layout: schema
name: Finout Cost Query
properties_list:
- description: The ID of the Finout View to query.
  name: viewId
  type: string
- description: Optional date range for the query. Must either be fully specified or omitted entirely.
  name: date
  type: object
- description: A filter object used to narrow query results, supporting logical AND/OR grouping and various operators.
  name: filter
  type: object
provider_name: Finout
provider_slug: finout
schema_file: json-schema/cost-query.json
slug: cost-query
source_filename: cost-query.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/finout/blob/main/json-schema/cost-query.json\",\n  \"title\": \"Finout Cost Query\",\n  \"description\": \"A cost query request used to analyze cloud spend using user-defined Finout Views, supporting date ranges and filters for granular cost insights.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"viewId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Finout View to query.\"\n    },\n    \"date\": {\n      \"type\": \"object\",\n      \"description\": \"Optional date range for the query. Must either be fully specified or omitted entirely.\",\n      \"properties\": {\n        \"unixTimeMillSecondsStart\": {\n          \"type\": \"integer\",\n          \"description\": \"Start of the date range in Unix milliseconds (UTC).\"\n        },\n        \"unixTimeMillSecondsEnd\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"End of the date range in Unix milliseconds (UTC).\"\n        }\n      }\n    },\n    \"filter\": {\n      \"type\": \"object\",\n      \"description\": \"A filter object used to narrow query results, supporting logical AND/OR grouping and various operators.\",\n      \"properties\": {\n        \"costCenter\": {\n          \"type\": \"string\",\n          \"description\": \"The cost center to filter on (e.g., AWS, GCP, Azure).\"\n        },\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The MegaBill key to filter by.\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name for the filter field.\"\n        },\n        \"operator\": {\n          \"type\": \"string\",\n          \"description\": \"The filter operator.\",\n          \"enum\": [\"oneOf\", \"notOneOf\", \"is\", \"isNot\", \"contains\", \"notContains\", \"exists\", \"notExists\"]\n        },\n        \"value\": {\n        \
  \  \"description\": \"The value or values to match against.\",\n          \"oneOf\": [\n            { \"type\": \"string\" },\n            { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n          ]\n        }\n      }\n    }\n  },\n  \"required\": [\"viewId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/finout/refs/heads/main/json-schema/cost-query.json
tags:
- Budgets
- Costs
- FinOps
title: Finout Cost Query
---
