---
description: SecretRef struct for a reference to a secret key.
layout: schema
name: v1alpha1SecretRef
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: secretName
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-secret-ref-schema.json
slug: argo-cd-v1alpha1-secret-ref
source_filename: argo-cd-v1alpha1-secret-ref-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-secret-ref-schema.json\",\n  \"title\": \"v1alpha1SecretRef\",\n  \"description\": \"SecretRef struct for a reference to a secret key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"secretName\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-secret-ref-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SecretRef
---
