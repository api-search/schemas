---
description: ''
layout: schema
name: ServiceDiscoveryConfiguration
properties_list:
- description: ''
  name: cache_disabled
  type: boolean
- description: ''
  name: cache_timeout
  type: integer
- description: ''
  name: data_path
  type: string
- description: ''
  name: endpoint_returns_list
  type: boolean
- description: ''
  name: parent_data_path
  type: string
- description: ''
  name: port_data_path
  type: string
- description: ''
  name: query_endpoint
  type: string
- description: ''
  name: target_path
  type: string
- description: ''
  name: use_discovery_service
  type: boolean
- description: ''
  name: use_nested_query
  type: boolean
- description: ''
  name: use_target_list
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-service-discovery-configuration-schema.json
slug: tyk-gateway-service-discovery-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceDiscoveryConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cache_disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"cache_timeout\": {\n      \"type\": \"integer\"\n    },\n    \"data_path\": {\n      \"type\": \"string\"\n    },\n    \"endpoint_returns_list\": {\n      \"type\": \"boolean\"\n    },\n    \"parent_data_path\": {\n      \"type\": \"string\"\n    },\n    \"port_data_path\": {\n      \"type\": \"string\"\n    },\n    \"query_endpoint\": {\n      \"type\": \"string\"\n    },\n    \"target_path\": {\n      \"type\": \"string\"\n    },\n    \"use_discovery_service\": {\n      \"type\": \"boolean\"\n    },\n    \"use_nested_query\": {\n      \"type\": \"boolean\"\n    },\n    \"use_target_list\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-service-discovery-configuration-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: ServiceDiscoveryConfiguration
---
