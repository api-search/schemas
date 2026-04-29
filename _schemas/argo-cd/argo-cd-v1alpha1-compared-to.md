---
description: v1alpha1ComparedTo schema from Argo CD API
layout: schema
name: v1alpha1ComparedTo
properties_list:
- description: ''
  name: destination
  type: object
- description: ''
  name: ignoreDifferences
  type: array
- description: ''
  name: source
  type: object
- description: ''
  name: sources
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-compared-to-schema.json
slug: argo-cd-v1alpha1-compared-to
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-compared-to-schema.json\",\n  \"title\": \"v1alpha1ComparedTo\",\n  \"description\": \"v1alpha1ComparedTo schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destination\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationDestination\"\n    },\n    \"ignoreDifferences\": {\n      \"type\": \"array\",\n      \"title\": \"IgnoreDifferences is a reference to the application's ignored differences used for comparison\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ResourceIgnoreDifferences\"\n      }\n    },\n    \"source\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSource\"\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"title\": \"Sources is a reference to the application's multiple sources used for comparison\",\n  \
  \    \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationSource\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-compared-to-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ComparedTo
---
