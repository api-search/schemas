---
description: API_Entities_Cluster model
layout: schema
name: API_Entities_Cluster
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: domain
  type: string
- description: ''
  name: enabled
  type: string
- description: ''
  name: managed
  type: string
- description: ''
  name: provider_type
  type: string
- description: ''
  name: platform_type
  type: string
- description: ''
  name: environment_scope
  type: string
- description: ''
  name: cluster_type
  type: string
- description: ''
  name: namespace_per_environment
  type: string
- description: ''
  name: user
  type: object
- description: ''
  name: platform_kubernetes
  type: object
- description: ''
  name: provider_gcp
  type: object
- description: ''
  name: management_project
  type: object
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-api-v4-admin-api_entities_cluster-schema.json
slug: gitlab-api-v4-admin-api_entities_cluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-admin-api_entities_cluster-schema.json\",\n  \"title\": \"API_Entities_Cluster\",\n  \"description\": \"API_Entities_Cluster model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"123456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Project\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"enabled\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"managed\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"provider_type\": {\n      \"type\": \"string\",\n     \
  \ \"example\": \"example_value\"\n    },\n    \"platform_type\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"environment_scope\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"cluster_type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"namespace_per_environment\": {\n      \"type\": \"string\",\n      \"example\": \"Example Project\"\n    },\n    \"user\": {\n      \"$ref\": \"#/components/schemas/API_Entities_UserBasic\"\n    },\n    \"platform_kubernetes\": {\n      \"$ref\": \"#/components/schemas/API_Entities_Platform_Kubernetes\"\n    },\n    \"provider_gcp\": {\n      \"$ref\": \"#/components/schemas/API_Entities_Provider_Gcp\"\n    },\n    \"management_project\": {\n      \"$ref\": \"#/components/schemas/API_Entities_ProjectIdentity\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-admin-api_entities_cluster-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_Cluster
---
