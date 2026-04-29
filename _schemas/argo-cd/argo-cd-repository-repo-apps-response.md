---
description: repositoryRepoAppsResponse schema from Argo CD API
layout: schema
name: repositoryRepoAppsResponse
properties_list:
- description: ''
  name: items
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-repository-repo-apps-response-schema.json
slug: argo-cd-repository-repo-apps-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-repo-apps-response-schema.json\",\n  \"title\": \"repositoryRepoAppsResponse\",\n  \"description\": \"repositoryRepoAppsResponse schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/repositoryAppInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-repo-apps-response-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: repositoryRepoAppsResponse
---
