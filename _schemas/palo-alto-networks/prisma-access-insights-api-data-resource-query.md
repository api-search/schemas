---
description: Query parameters for a data resource request
layout: schema
name: DataResourceQuery
properties_list:
- description: Query definition including filters and time range
  name: query
  type: object
- description: Maximum number of results to return
  name: count
  type: integer
- description: Histogram aggregation configuration
  name: histogram
  type: object
- description: Properties to group results by
  name: group_by
  type: array
- description: Sort configuration for results
  name: sort
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-insights-api-data-resource-query-schema.json
slug: prisma-access-insights-api-data-resource-query
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataResourceQuery\",\n  \"description\": \"Query parameters for a data resource request\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-insights-api-data-resource-query-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"object\",\n      \"description\": \"Query definition including filters and time range\",\n      \"properties\": {\n        \"properties\": {\n          \"type\": \"object\",\n          \"description\": \"Property filters for the query\",\n          \"properties\": {\n            \"time_range\": {\n              \"type\": \"object\",\n              \"description\": \"Time range specification for the query\",\n              \"required\": [\n                \"type\"\n              ],\n              \"properties\": {\n                \"type\": {\n        \
  \          \"type\": \"string\",\n                  \"description\": \"Type of time range (absolute or relative)\",\n                  \"enum\": [\n                    \"ABSOLUTE\",\n                    \"RELATIVE\"\n                  ]\n                },\n                \"value\": {\n                  \"type\": \"object\",\n                  \"description\": \"Time range value (required for ABSOLUTE type)\",\n                  \"properties\": {\n                    \"from\": {\n                      \"type\": \"string\",\n                      \"format\": \"date-time\",\n                      \"description\": \"Start of the time range (ISO 8601)\"\n                    },\n                    \"to\": {\n                      \"type\": \"string\",\n                      \"format\": \"date-time\",\n                      \"description\": \"End of the time range (ISO 8601)\"\n                    }\n                  }\n                },\n                \"last\": {\n                  \"\
  type\": \"object\",\n                  \"description\": \"Relative time range (required for RELATIVE type)\",\n                  \"properties\": {\n                    \"units\": {\n                      \"type\": \"string\",\n                      \"enum\": [\n                        \"HOURS\",\n                        \"DAYS\",\n                        \"WEEKS\"\n                      ],\n                      \"description\": \"Unit of time for relative range\"\n                    },\n                    \"value\": {\n                      \"type\": \"integer\",\n                      \"description\": \"Number of units for relative range\"\n                    }\n                  }\n                }\n              }\n            },\n            \"filter\": {\n              \"type\": \"object\",\n              \"description\": \"Filter criteria for the data resource query\",\n              \"properties\": {\n                \"operator\": {\n                  \"type\": \"string\",\n\
  \                  \"description\": \"Logical operator for combining filter rules\",\n                  \"enum\": [\n                    \"AND\",\n                    \"OR\"\n                  ]\n                },\n                \"rules\": {\n                  \"type\": \"array\",\n                  \"description\": \"List of filter rules\",\n                  \"items\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"property\": {\n                        \"type\": \"string\",\n                        \"description\": \"Property name to filter on\"\n                      },\n                      \"operator\": {\n                        \"type\": \"string\",\n                        \"description\": \"Comparison operator\",\n                        \"enum\": [\n                          \"equals\",\n                          \"not_equals\",\n                          \"contains\",\n                          \"in\",\n    \
  \                      \"not_in\",\n                          \"greater_than\",\n                          \"less_than\"\n                        ]\n                      },\n                      \"values\": {\n                        \"type\": \"array\",\n                        \"description\": \"Values to match against\",\n                        \"items\": {\n                          \"type\": \"string\"\n                        }\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of results to return\",\n      \"minimum\": 1,\n      \"maximum\": 1000,\n      \"default\": 100\n    },\n    \"histogram\": {\n      \"type\": \"object\",\n      \"description\": \"Histogram aggregation configuration\",\n      \"properties\": {\n        \"property\": {\n          \"type\": \"string\",\n   \
  \       \"description\": \"Property to aggregate over\"\n        },\n        \"enabledGranularity\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"15_MIN\",\n            \"1_HOUR\",\n            \"1_DAY\"\n          ],\n          \"description\": \"Time granularity for histogram buckets\"\n        }\n      }\n    },\n    \"group_by\": {\n      \"type\": \"array\",\n      \"description\": \"Properties to group results by\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"sort\": {\n      \"type\": \"object\",\n      \"description\": \"Sort configuration for results\",\n      \"properties\": {\n        \"order\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"asc\",\n            \"desc\"\n          ]\n        },\n        \"property\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-insights-api-data-resource-query-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DataResourceQuery
---
