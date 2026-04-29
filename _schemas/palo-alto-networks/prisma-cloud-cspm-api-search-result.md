---
description: SearchResult schema from Palo Alto Networks Prisma Cloud CSPM API
layout: schema
name: SearchResult
properties_list:
- description: Cloud provider type for the search results.
  name: cloudType
  type: string
- description: RQL query that was executed.
  name: query
  type: string
- description: ''
  name: data
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-cspm-api-search-result-schema.json
slug: prisma-cloud-cspm-api-search-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchResult\",\n  \"description\": \"SearchResult schema from Palo Alto Networks Prisma Cloud CSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-search-result-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cloudType\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud provider type for the search results.\"\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"RQL query that was executed.\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"totalRows\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of matching resources.\"\n        },\n        \"items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\"\
  : {\n              \"id\": {\n                \"type\": \"string\"\n              },\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"cloudType\": {\n                \"type\": \"string\"\n              },\n              \"accountId\": {\n                \"type\": \"string\"\n              },\n              \"accountName\": {\n                \"type\": \"string\"\n              },\n              \"regionId\": {\n                \"type\": \"string\"\n              },\n              \"resourceType\": {\n                \"type\": \"string\"\n              },\n              \"overallPassed\": {\n                \"type\": \"boolean\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-search-result-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SearchResult
---
