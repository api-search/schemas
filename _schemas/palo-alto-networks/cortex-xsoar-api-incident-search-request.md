---
description: IncidentSearchRequest schema from Palo Alto Networks Cortex XSOAR REST API
layout: schema
name: IncidentSearchRequest
properties_list:
- description: Structured filter criteria for the incident search.
  name: filter
  type: object
- description: ''
  name: fromDate
  type: string
- description: ''
  name: toDate
  type: string
- description: ''
  name: size
  type: integer
- description: ''
  name: page
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsoar-api-incident-search-request-schema.json
slug: cortex-xsoar-api-incident-search-request
source_filename: cortex-xsoar-api-incident-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IncidentSearchRequest\",\n  \"description\": \"IncidentSearchRequest schema from Palo Alto Networks Cortex XSOAR REST API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-incident-search-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filter\": {\n      \"type\": \"object\",\n      \"description\": \"Structured filter criteria for the incident search.\",\n      \"properties\": {\n        \"query\": {\n          \"type\": \"string\",\n          \"description\": \"Lucene query string (e.g., status:Active severity:High).\"\n        },\n        \"status\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"integer\"\n          }\n        },\n        \"sort\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n    \
  \        \"properties\": {\n              \"field\": {\n                \"type\": \"string\"\n              },\n              \"asc\": {\n                \"type\": \"boolean\"\n              }\n            }\n          }\n        },\n        \"period\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"byFrom\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\"\n            },\n            \"byTo\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\"\n            }\n          }\n        }\n      }\n    },\n    \"fromDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"toDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"default\": 10,\n      \"maximum\": 100\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"default\": 0\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-incident-search-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: IncidentSearchRequest
---
