---
description: ''
layout: schema
name: OpenCost Asset
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: totalCost
  type: number
- description: ''
  name: cpuCost
  type: number
- description: ''
  name: ramCost
  type: number
- description: ''
  name: providerID
  type: string
- description: ''
  name: window
  type: object
provider_name: OpenCost
provider_slug: opencost
schema_file: json-schema/opencost-asset-schema.json
slug: opencost-asset
source_filename: opencost-asset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/opencost/json-schema/opencost-asset-schema.json\",\n  \"title\": \"OpenCost Asset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\"type\": \"string\"},\n    \"totalCost\": {\"type\": \"number\"},\n    \"cpuCost\": {\"type\": \"number\"},\n    \"ramCost\": {\"type\": \"number\"},\n    \"providerID\": {\"type\": \"string\"},\n    \"window\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start\": {\"type\": \"string\", \"format\": \"date-time\"},\n        \"end\": {\"type\": \"string\", \"format\": \"date-time\"}\n      }\n    }\n  },\n  \"required\": [\"type\", \"totalCost\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/opencost/refs/heads/main/json-schema/opencost-asset-schema.json
tags:
- Cloud Cost Management
- CNCF
- FinOps
- Kubernetes
- Observability
title: OpenCost Asset
---
