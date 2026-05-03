---
description: ''
layout: schema
name: OpenCost Allocation
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: cpuCost
  type: number
- description: ''
  name: cpuCoreUsageAverage
  type: number
- description: ''
  name: ramCost
  type: number
- description: ''
  name: ramByteUsageAverage
  type: number
- description: ''
  name: pvCost
  type: number
- description: ''
  name: networkCost
  type: number
- description: ''
  name: sharedCost
  type: number
- description: ''
  name: externalCost
  type: number
- description: ''
  name: totalCost
  type: number
- description: ''
  name: minutes
  type: number
- description: ''
  name: window
  type: object
- description: ''
  name: properties
  type: object
provider_name: OpenCost
provider_slug: opencost
schema_file: json-schema/opencost-allocation-schema.json
slug: opencost-allocation
source_filename: opencost-allocation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/opencost/json-schema/opencost-allocation-schema.json\",\n  \"title\": \"OpenCost Allocation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\"type\": \"string\"},\n    \"cpuCost\": {\"type\": \"number\"},\n    \"cpuCoreUsageAverage\": {\"type\": \"number\"},\n    \"ramCost\": {\"type\": \"number\"},\n    \"ramByteUsageAverage\": {\"type\": \"number\"},\n    \"pvCost\": {\"type\": \"number\"},\n    \"networkCost\": {\"type\": \"number\"},\n    \"sharedCost\": {\"type\": \"number\"},\n    \"externalCost\": {\"type\": \"number\"},\n    \"totalCost\": {\"type\": \"number\"},\n    \"minutes\": {\"type\": \"number\"},\n    \"window\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start\": {\"type\": \"string\", \"format\": \"date-time\"},\n        \"end\": {\"type\": \"string\", \"format\": \"date-time\"}\n      }\n    },\n    \"\
  properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\"type\": \"string\"}\n    }\n  },\n  \"required\": [\"name\", \"totalCost\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/opencost/refs/heads/main/json-schema/opencost-allocation-schema.json
tags:
- Cloud Cost Management
- CNCF
- FinOps
- Kubernetes
- Observability
title: OpenCost Allocation
---
