---
description: ''
layout: schema
name: ServiceDiscovery
properties_list:
- description: ''
  name: cacheTimeout
  type: integer
- description: ''
  name: dataPath
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: endpointReturnsList
  type: boolean
- description: ''
  name: parentDataPath
  type: string
- description: ''
  name: portDataPath
  type: string
- description: ''
  name: queryEndpoint
  type: string
- description: ''
  name: targetPath
  type: string
- description: ''
  name: useNestedQuery
  type: boolean
- description: ''
  name: useTargetList
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-service-discovery-schema.json
slug: tyk-gateway-service-discovery
source_filename: tyk-gateway-service-discovery-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceDiscovery\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cacheTimeout\": {\n      \"type\": \"integer\"\n    },\n    \"dataPath\": {\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"endpointReturnsList\": {\n      \"type\": \"boolean\"\n    },\n    \"parentDataPath\": {\n      \"type\": \"string\"\n    },\n    \"portDataPath\": {\n      \"type\": \"string\"\n    },\n    \"queryEndpoint\": {\n      \"type\": \"string\"\n    },\n    \"targetPath\": {\n      \"type\": \"string\"\n    },\n    \"useNestedQuery\": {\n      \"type\": \"boolean\"\n    },\n    \"useTargetList\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-service-discovery-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: ServiceDiscovery
---
