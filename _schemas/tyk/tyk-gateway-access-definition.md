---
description: ''
layout: schema
name: AccessDefinition
properties_list:
- description: ''
  name: allowance_scope
  type: string
- description: ''
  name: allowed_types
  type: array
- description: ''
  name: allowed_urls
  type: array
- description: ''
  name: api_id
  type: string
- description: ''
  name: api_name
  type: string
- description: ''
  name: disable_introspection
  type: boolean
- description: ''
  name: field_access_rights
  type: array
- description: ''
  name: restricted_types
  type: array
- description: ''
  name: versions
  type: array
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-access-definition-schema.json
slug: tyk-gateway-access-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccessDefinition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowance_scope\": {\n      \"type\": \"string\"\n    },\n    \"allowed_types\": {\n      \"type\": \"array\"\n    },\n    \"allowed_urls\": {\n      \"type\": \"array\"\n    },\n    \"api_id\": {\n      \"type\": \"string\"\n    },\n    \"api_name\": {\n      \"type\": \"string\"\n    },\n    \"disable_introspection\": {\n      \"type\": \"boolean\"\n    },\n    \"field_access_rights\": {\n      \"type\": \"array\"\n    },\n    \"restricted_types\": {\n      \"type\": \"array\"\n    },\n    \"versions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-access-definition-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: AccessDefinition
---
