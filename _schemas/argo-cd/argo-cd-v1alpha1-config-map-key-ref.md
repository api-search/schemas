---
description: ConfigMapKeyRef struct for a reference to a configmap key.
layout: schema
name: v1alpha1ConfigMapKeyRef
properties_list:
- description: ''
  name: configMapName
  type: string
- description: ''
  name: key
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-config-map-key-ref-schema.json
slug: argo-cd-v1alpha1-config-map-key-ref
source_filename: argo-cd-v1alpha1-config-map-key-ref-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-config-map-key-ref-schema.json\",\n  \"title\": \"v1alpha1ConfigMapKeyRef\",\n  \"description\": \"ConfigMapKeyRef struct for a reference to a configmap key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configMapName\": {\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-config-map-key-ref-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ConfigMapKeyRef
---
