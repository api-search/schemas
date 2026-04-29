---
description: v1alpha1Operation schema from Argo CD API
layout: schema
name: v1alpha1Operation
properties_list:
- description: ''
  name: info
  type: array
- description: ''
  name: initiatedBy
  type: object
- description: ''
  name: retry
  type: object
- description: ''
  name: sync
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-operation-schema.json
slug: argo-cd-v1alpha1-operation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-operation-schema.json\",\n  \"title\": \"v1alpha1Operation\",\n  \"description\": \"v1alpha1Operation schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"info\": {\n      \"type\": \"array\",\n      \"title\": \"Info is a list of informational items for this operation\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1Info\"\n      }\n    },\n    \"initiatedBy\": {\n      \"$ref\": \"#/definitions/v1alpha1OperationInitiator\"\n    },\n    \"retry\": {\n      \"$ref\": \"#/definitions/v1alpha1RetryStrategy\"\n    },\n    \"sync\": {\n      \"$ref\": \"#/definitions/v1alpha1SyncOperation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-operation-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1Operation
---
