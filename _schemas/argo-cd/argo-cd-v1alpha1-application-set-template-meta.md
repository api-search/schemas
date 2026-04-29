---
description: v1alpha1ApplicationSetTemplateMeta schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSetTemplateMeta
properties_list:
- description: ''
  name: annotations
  type: object
- description: ''
  name: finalizers
  type: array
- description: ''
  name: labels
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-template-meta-schema.json
slug: argo-cd-v1alpha1-application-set-template-meta
source_filename: argo-cd-v1alpha1-application-set-template-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-template-meta-schema.json\",\n  \"title\": \"v1alpha1ApplicationSetTemplateMeta\",\n  \"description\": \"v1alpha1ApplicationSetTemplateMeta schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"annotations\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"finalizers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-template-meta-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetTemplateMeta
---
