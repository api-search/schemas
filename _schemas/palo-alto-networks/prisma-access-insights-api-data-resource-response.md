---
description: Response containing data resource query results
layout: schema
name: DataResourceResponse
properties_list:
- description: Response metadata
  name: header
  type: object
- description: Array of result records
  name: data
  type: array
- description: Total number of records matching the query
  name: count
  type: integer
- description: Pagination information
  name: pagination
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-insights-api-data-resource-response-schema.json
slug: prisma-access-insights-api-data-resource-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataResourceResponse\",\n  \"description\": \"Response containing data resource query results\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-insights-api-data-resource-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"header\": {\n      \"type\": \"object\",\n      \"description\": \"Response metadata\",\n      \"properties\": {\n        \"requestId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique request identifier\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"success\",\n            \"failed\",\n            \"partial\"\n          ]\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"data\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"Array of result records\",\n      \"items\": {\n        \"type\": \"object\",\n        \"additionalProperties\": true\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of records matching the query\"\n    },\n    \"pagination\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information\",\n      \"properties\": {\n        \"offset\": {\n          \"type\": \"integer\",\n          \"description\": \"Current result offset\"\n        },\n        \"limit\": {\n          \"type\": \"integer\",\n          \"description\": \"Page size\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-insights-api-data-resource-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DataResourceResponse
---
