---
description: v1alpha1AppProject schema from Argo CD API
layout: schema
name: v1alpha1AppProject
properties_list:
- description: ''
  name: metadata
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: status
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-app-project-schema.json
slug: argo-cd-v1alpha1-app-project
source_filename: argo-cd-v1alpha1-app-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-app-project-schema.json\",\n  \"title\": \"v1alpha1AppProject\",\n  \"description\": \"v1alpha1AppProject schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata\": {\n      \"$ref\": \"#/definitions/v1ObjectMeta\"\n    },\n    \"spec\": {\n      \"$ref\": \"#/definitions/v1alpha1AppProjectSpec\"\n    },\n    \"status\": {\n      \"$ref\": \"#/definitions/v1alpha1AppProjectStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-app-project-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1AppProject
---
