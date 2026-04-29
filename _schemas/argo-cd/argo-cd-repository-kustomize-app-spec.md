---
description: repositoryKustomizeAppSpec schema from Argo CD API
layout: schema
name: repositoryKustomizeAppSpec
properties_list:
- description: images is a list of available images.
  name: images
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-repository-kustomize-app-spec-schema.json
slug: argo-cd-repository-kustomize-app-spec
source_filename: argo-cd-repository-kustomize-app-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-kustomize-app-spec-schema.json\",\n  \"title\": \"repositoryKustomizeAppSpec\",\n  \"description\": \"repositoryKustomizeAppSpec schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"images\": {\n      \"description\": \"images is a list of available images.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-kustomize-app-spec-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: repositoryKustomizeAppSpec
---
