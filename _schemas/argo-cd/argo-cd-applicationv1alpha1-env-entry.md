---
description: applicationv1alpha1EnvEntry schema from Argo CD API
layout: schema
name: applicationv1alpha1EnvEntry
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: value
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-applicationv1alpha1-env-entry-schema.json
slug: argo-cd-applicationv1alpha1-env-entry
source_filename: argo-cd-applicationv1alpha1-env-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-applicationv1alpha1-env-entry-schema.json\",\n  \"title\": \"applicationv1alpha1EnvEntry\",\n  \"description\": \"applicationv1alpha1EnvEntry schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name is the name of the variable, usually expressed in uppercase\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"title\": \"Value is the value of the variable\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-applicationv1alpha1-env-entry-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: applicationv1alpha1EnvEntry
---
