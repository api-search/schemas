---
description: v1alpha1KustomizeSelector schema from Argo CD API
layout: schema
name: v1alpha1KustomizeSelector
properties_list:
- description: ''
  name: annotationSelector
  type: string
- description: ''
  name: labelSelector
  type: string
- description: ''
  name: resId
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-kustomize-selector-schema.json
slug: argo-cd-v1alpha1-kustomize-selector
source_filename: argo-cd-v1alpha1-kustomize-selector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-kustomize-selector-schema.json\",\n  \"title\": \"v1alpha1KustomizeSelector\",\n  \"description\": \"v1alpha1KustomizeSelector schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"annotationSelector\": {\n      \"type\": \"string\"\n    },\n    \"labelSelector\": {\n      \"type\": \"string\"\n    },\n    \"resId\": {\n      \"$ref\": \"#/definitions/v1alpha1KustomizeResId\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-kustomize-selector-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1KustomizeSelector
---
