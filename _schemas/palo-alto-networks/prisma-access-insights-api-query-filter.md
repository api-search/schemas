---
description: Filter criteria for the data resource query
layout: schema
name: QueryFilter
properties_list:
- description: Logical operator for combining filter rules
  name: operator
  type: string
- description: List of filter rules
  name: rules
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-insights-api-query-filter-schema.json
slug: prisma-access-insights-api-query-filter
source_filename: prisma-access-insights-api-query-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryFilter\",\n  \"description\": \"Filter criteria for the data resource query\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-insights-api-query-filter-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operator\": {\n      \"type\": \"string\",\n      \"description\": \"Logical operator for combining filter rules\",\n      \"enum\": [\n        \"AND\",\n        \"OR\"\n      ]\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"description\": \"List of filter rules\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"property\": {\n            \"type\": \"string\",\n            \"description\": \"Property name to filter on\"\n          },\n          \"operator\": {\n            \"type\": \"string\",\n            \"description\": \"Comparison\
  \ operator\",\n            \"enum\": [\n              \"equals\",\n              \"not_equals\",\n              \"contains\",\n              \"in\",\n              \"not_in\",\n              \"greater_than\",\n              \"less_than\"\n            ]\n          },\n          \"values\": {\n            \"type\": \"array\",\n            \"description\": \"Values to match against\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-insights-api-query-filter-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: QueryFilter
---
