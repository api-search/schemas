---
description: Schema describing an OpenSearch Security plugin role definition.
layout: schema
name: OpenSearch Security Role
properties_list:
- description: Cluster-level permissions or action group references.
  name: cluster_permissions
  type: array
- description: ''
  name: index_permissions
  type: array
- description: ''
  name: tenant_permissions
  type: array
- description: ''
  name: description
  type: string
- description: ''
  name: reserved
  type: boolean
- description: ''
  name: hidden
  type: boolean
- description: ''
  name: static
  type: boolean
provider_name: OpenSearch
provider_slug: opensearch
schema_file: json-schema/opensearch-role-schema.json
slug: opensearch-role
source_filename: opensearch-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/json-schema/opensearch-role-schema.json\",\n  \"title\": \"OpenSearch Security Role\",\n  \"description\": \"Schema describing an OpenSearch Security plugin role definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cluster_permissions\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Cluster-level permissions or action group references.\"\n    },\n    \"index_permissions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"index_patterns\": {\n            \"type\": \"array\",\n            \"items\": { \"type\": \"string\" }\n          },\n          \"dls\": {\n            \"type\": \"string\",\n            \"description\": \"Document-level security query.\"\n          },\n         \
  \ \"fls\": {\n            \"type\": \"array\",\n            \"items\": { \"type\": \"string\" },\n            \"description\": \"Field-level security inclusions or exclusions.\"\n          },\n          \"masked_fields\": {\n            \"type\": \"array\",\n            \"items\": { \"type\": \"string\" }\n          },\n          \"allowed_actions\": {\n            \"type\": \"array\",\n            \"items\": { \"type\": \"string\" }\n          }\n        },\n        \"required\": [\"index_patterns\", \"allowed_actions\"]\n      }\n    },\n    \"tenant_permissions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"tenant_patterns\": {\n            \"type\": \"array\",\n            \"items\": { \"type\": \"string\" }\n          },\n          \"allowed_actions\": {\n            \"type\": \"array\",\n            \"items\": { \"type\": \"string\" }\n          }\n        },\n        \"required\": [\"tenant_patterns\",\
  \ \"allowed_actions\"]\n      }\n    },\n    \"description\": { \"type\": \"string\" },\n    \"reserved\": { \"type\": \"boolean\" },\n    \"hidden\": { \"type\": \"boolean\" },\n    \"static\": { \"type\": \"boolean\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/json-schema/opensearch-role-schema.json
tags:
- Search
- Analytics
- Observability
- Open Source
- Security
title: OpenSearch Security Role
---
