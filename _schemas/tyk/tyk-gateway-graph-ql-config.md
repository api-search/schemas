---
description: ''
layout: schema
name: GraphQLConfig
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: execution_mode
  type: string
- description: ''
  name: last_schema_update
  type: string
- description: ''
  name: schema
  type: string
- description: ''
  name: type_field_configurations
  type: array
- description: ''
  name: version
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-graph-ql-config-schema.json
slug: tyk-gateway-graph-ql-config
source_filename: tyk-gateway-graph-ql-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GraphQLConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"execution_mode\": {\n      \"type\": \"string\"\n    },\n    \"last_schema_update\": {\n      \"type\": \"string\"\n    },\n    \"schema\": {\n      \"type\": \"string\"\n    },\n    \"type_field_configurations\": {\n      \"type\": \"array\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-graph-ql-config-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: GraphQLConfig
---
