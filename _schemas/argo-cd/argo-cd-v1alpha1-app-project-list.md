---
description: v1alpha1AppProjectList schema from Argo CD API
layout: schema
name: v1alpha1AppProjectList
properties_list:
- description: ''
  name: items
  type: array
- description: ''
  name: metadata
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-app-project-list-schema.json
slug: argo-cd-v1alpha1-app-project-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-app-project-list-schema.json\",\n  \"title\": \"v1alpha1AppProjectList\",\n  \"description\": \"v1alpha1AppProjectList schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1AppProject\"\n      }\n    },\n    \"metadata\": {\n      \"$ref\": \"#/definitions/v1ListMeta\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-app-project-list-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1AppProjectList
---
