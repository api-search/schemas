---
description: v1alpha1KustomizeVersion schema from Argo CD API
layout: schema
name: v1alpha1KustomizeVersion
properties_list:
- description: ''
  name: buildOptions
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: path
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-kustomize-version-schema.json
slug: argo-cd-v1alpha1-kustomize-version
source_filename: argo-cd-v1alpha1-kustomize-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-kustomize-version-schema.json\",\n  \"title\": \"v1alpha1KustomizeVersion\",\n  \"description\": \"v1alpha1KustomizeVersion schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"buildOptions\": {\n      \"type\": \"string\",\n      \"title\": \"BuildOptions that are specific to a Kustomize version\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name holds Kustomize version name\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"title\": \"Path holds the corresponding binary path\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-kustomize-version-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1KustomizeVersion
---
