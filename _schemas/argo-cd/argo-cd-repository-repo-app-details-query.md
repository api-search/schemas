---
description: repositoryRepoAppDetailsQuery schema from Argo CD API
layout: schema
name: repositoryRepoAppDetailsQuery
properties_list:
- description: ''
  name: appName
  type: string
- description: ''
  name: appProject
  type: string
- description: ''
  name: source
  type: object
- description: ''
  name: sourceIndex
  type: integer
- description: ''
  name: versionId
  type: integer
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-repository-repo-app-details-query-schema.json
slug: argo-cd-repository-repo-app-details-query
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-repo-app-details-query-schema.json\",\n  \"title\": \"repositoryRepoAppDetailsQuery\",\n  \"description\": \"repositoryRepoAppDetailsQuery schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appName\": {\n      \"type\": \"string\"\n    },\n    \"appProject\": {\n      \"type\": \"string\"\n    },\n    \"source\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSource\"\n    },\n    \"sourceIndex\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"title\": \"source index (for multi source apps)\"\n    },\n    \"versionId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"title\": \"versionId from historical data (for multi source apps)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-repo-app-details-query-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: repositoryRepoAppDetailsQuery
---
