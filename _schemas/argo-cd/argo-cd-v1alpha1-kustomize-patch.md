---
description: v1alpha1KustomizePatch schema from Argo CD API
layout: schema
name: v1alpha1KustomizePatch
properties_list:
- description: ''
  name: options
  type: object
- description: ''
  name: patch
  type: string
- description: ''
  name: path
  type: string
- description: ''
  name: target
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-kustomize-patch-schema.json
slug: argo-cd-v1alpha1-kustomize-patch
source_filename: argo-cd-v1alpha1-kustomize-patch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-kustomize-patch-schema.json\",\n  \"title\": \"v1alpha1KustomizePatch\",\n  \"description\": \"v1alpha1KustomizePatch schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"options\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"boolean\"\n      }\n    },\n    \"patch\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"target\": {\n      \"$ref\": \"#/definitions/v1alpha1KustomizeSelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-kustomize-patch-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1KustomizePatch
---
