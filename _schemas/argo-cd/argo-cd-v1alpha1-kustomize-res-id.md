---
description: v1alpha1KustomizeResId schema from Argo CD API
layout: schema
name: v1alpha1KustomizeResId
properties_list:
- description: ''
  name: gvk
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-kustomize-res-id-schema.json
slug: argo-cd-v1alpha1-kustomize-res-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-kustomize-res-id-schema.json\",\n  \"title\": \"v1alpha1KustomizeResId\",\n  \"description\": \"v1alpha1KustomizeResId schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gvk\": {\n      \"$ref\": \"#/definitions/v1alpha1KustomizeGvk\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-kustomize-res-id-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1KustomizeResId
---
