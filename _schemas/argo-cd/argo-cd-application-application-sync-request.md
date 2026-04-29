---
description: applicationApplicationSyncRequest schema from Argo CD API
layout: schema
name: applicationApplicationSyncRequest
properties_list:
- description: ''
  name: appNamespace
  type: string
- description: ''
  name: dryRun
  type: boolean
- description: ''
  name: infos
  type: array
- description: ''
  name: manifests
  type: array
- description: ''
  name: name
  type: string
- description: ''
  name: project
  type: string
- description: ''
  name: prune
  type: boolean
- description: ''
  name: resources
  type: array
- description: ''
  name: retryStrategy
  type: object
- description: ''
  name: revision
  type: string
- description: ''
  name: revisions
  type: array
- description: ''
  name: sourcePositions
  type: array
- description: ''
  name: strategy
  type: object
- description: ''
  name: syncOptions
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-application-application-sync-request-schema.json
slug: argo-cd-application-application-sync-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-application-sync-request-schema.json\",\n  \"title\": \"applicationApplicationSyncRequest\",\n  \"description\": \"applicationApplicationSyncRequest schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appNamespace\": {\n      \"type\": \"string\"\n    },\n    \"dryRun\": {\n      \"type\": \"boolean\"\n    },\n    \"infos\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1Info\"\n      }\n    },\n    \"manifests\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"project\": {\n      \"type\": \"string\"\n    },\n    \"prune\": {\n      \"type\": \"boolean\"\n    },\n    \"resources\": {\n      \"type\": \"array\"\
  ,\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1SyncOperationResource\"\n      }\n    },\n    \"retryStrategy\": {\n      \"$ref\": \"#/definitions/v1alpha1RetryStrategy\"\n    },\n    \"revision\": {\n      \"type\": \"string\"\n    },\n    \"revisions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"sourcePositions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"int64\"\n      }\n    },\n    \"strategy\": {\n      \"$ref\": \"#/definitions/v1alpha1SyncStrategy\"\n    },\n    \"syncOptions\": {\n      \"$ref\": \"#/definitions/applicationSyncOptions\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-application-sync-request-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: applicationApplicationSyncRequest
---
