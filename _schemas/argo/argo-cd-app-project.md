---
description: An Argo CD project providing logical grouping and RBAC for applications.
layout: schema
name: AppProject
properties_list:
- description: ''
  name: metadata
  type: object
- description: Project specification.
  name: spec
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-app-project-schema.json
slug: argo-cd-app-project
source_filename: argo-cd-app-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-app-project-schema.json\",\n  \"title\": \"AppProject\",\n  \"description\": \"An Argo CD project providing logical grouping and RBAC for applications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Project name.\"\n        }\n      }\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"description\": \"Project specification.\",\n      \"properties\": {\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable project description.\"\n        },\n        \"sourceRepos\": {\n          \"type\": \"array\",\n          \"description\": \"Allowed source repositories. Use '*' for any.\",\n       \
  \   \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"destinations\": {\n          \"type\": \"array\",\n          \"description\": \"Allowed destination clusters and namespaces.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"server\": {\n                \"type\": \"string\",\n                \"description\": \"Cluster server URL.\"\n              },\n              \"namespace\": {\n                \"type\": \"string\",\n                \"description\": \"Allowed namespace pattern.\"\n              }\n            }\n          }\n        },\n        \"clusterResourceWhitelist\": {\n          \"type\": \"array\",\n          \"description\": \"Allowed cluster-scoped resource types.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"group\": {\n                \"type\": \"string\"\n              },\n              \"kind\": {\n          \
  \      \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-app-project-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: AppProject
---
