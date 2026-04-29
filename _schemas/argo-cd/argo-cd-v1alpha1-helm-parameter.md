---
description: v1alpha1HelmParameter schema from Argo CD API
layout: schema
name: v1alpha1HelmParameter
properties_list:
- description: ''
  name: forceString
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: value
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-helm-parameter-schema.json
slug: argo-cd-v1alpha1-helm-parameter
source_filename: argo-cd-v1alpha1-helm-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-helm-parameter-schema.json\",\n  \"title\": \"v1alpha1HelmParameter\",\n  \"description\": \"v1alpha1HelmParameter schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"forceString\": {\n      \"type\": \"boolean\",\n      \"title\": \"ForceString determines whether to tell Helm to interpret booleans and numbers as strings\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name is the name of the Helm parameter\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"title\": \"Value is the value for the Helm parameter\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-helm-parameter-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1HelmParameter
---
