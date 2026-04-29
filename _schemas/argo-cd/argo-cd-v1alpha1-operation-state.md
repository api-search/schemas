---
description: v1alpha1OperationState schema from Argo CD API
layout: schema
name: v1alpha1OperationState
properties_list:
- description: ''
  name: finishedAt
  type: object
- description: Message holds any pertinent messages when attempting to perform operation (typically errors).
  name: message
  type: string
- description: ''
  name: operation
  type: object
- description: ''
  name: phase
  type: string
- description: ''
  name: retryCount
  type: integer
- description: ''
  name: startedAt
  type: object
- description: ''
  name: syncResult
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-operation-state-schema.json
slug: argo-cd-v1alpha1-operation-state
source_filename: argo-cd-v1alpha1-operation-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-operation-state-schema.json\",\n  \"title\": \"v1alpha1OperationState\",\n  \"description\": \"v1alpha1OperationState schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"finishedAt\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"message\": {\n      \"description\": \"Message holds any pertinent messages when attempting to perform operation (typically errors).\",\n      \"type\": \"string\"\n    },\n    \"operation\": {\n      \"$ref\": \"#/definitions/v1alpha1Operation\"\n    },\n    \"phase\": {\n      \"type\": \"string\",\n      \"title\": \"Phase is the current phase of the operation\"\n    },\n    \"retryCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"RetryCount contains time of operation retries\"\n    },\n\
  \    \"startedAt\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"syncResult\": {\n      \"$ref\": \"#/definitions/v1alpha1SyncOperationResult\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-operation-state-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1OperationState
---
