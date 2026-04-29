---
description: RepositoryList is a collection of Repositories.
layout: schema
name: v1alpha1RepositoryList
properties_list:
- description: ''
  name: items
  type: array
- description: ''
  name: metadata
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-repository-list-schema.json
slug: argo-cd-v1alpha1-repository-list
source_filename: argo-cd-v1alpha1-repository-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-repository-list-schema.json\",\n  \"title\": \"v1alpha1RepositoryList\",\n  \"description\": \"RepositoryList is a collection of Repositories.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1Repository\"\n      }\n    },\n    \"metadata\": {\n      \"$ref\": \"#/definitions/v1ListMeta\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-repository-list-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1RepositoryList
---
