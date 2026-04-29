---
description: ghes-config-nodes from GitHub API
layout: schema
name: ghes-config-nodes
properties_list:
- description: ''
  name: topology
  type: object
- description: ''
  name: nodes
  type: array
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-manage-ghes-config-nodes-schema.json
slug: github-manage-ghes-config-nodes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-manage-ghes-config-nodes-schema.json\",\n  \"title\": \"ghes-config-nodes\",\n  \"description\": \"ghes-config-nodes from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topology\": {\n      \"$ref\": \"#/components/schemas/ghes-cluster-topology\"\n    },\n    \"nodes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"hostname\": {\n            \"type\": \"string\"\n          },\n          \"uuid\": {\n            \"type\": \"string\"\n          },\n          \"replica\": {\n            \"type\": \"boolean\"\n          },\n          \"cluster_roles\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/ghes-cluster-roles\"\n            }\n          }\n    \
  \    }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-manage-ghes-config-nodes-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: ghes-config-nodes
---
