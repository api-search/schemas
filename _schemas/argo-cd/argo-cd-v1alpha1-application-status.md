---
description: v1alpha1ApplicationStatus schema from Argo CD API
layout: schema
name: v1alpha1ApplicationStatus
properties_list:
- description: ''
  name: conditions
  type: array
- description: ''
  name: controllerNamespace
  type: string
- description: ''
  name: health
  type: object
- description: ''
  name: history
  type: array
- description: ''
  name: observedAt
  type: object
- description: ''
  name: operationState
  type: object
- description: ''
  name: reconciledAt
  type: object
- description: ''
  name: resourceHealthSource
  type: string
- description: ''
  name: resources
  type: array
- description: ''
  name: sourceHydrator
  type: object
- description: ''
  name: sourceType
  type: string
- description: ''
  name: sourceTypes
  type: array
- description: ''
  name: summary
  type: object
- description: ''
  name: sync
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-status-schema.json
slug: argo-cd-v1alpha1-application-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-status-schema.json\",\n  \"title\": \"v1alpha1ApplicationStatus\",\n  \"description\": \"v1alpha1ApplicationStatus schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"conditions\": {\n      \"type\": \"array\",\n      \"title\": \"Conditions is a list of currently observed application conditions\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationCondition\"\n      }\n    },\n    \"controllerNamespace\": {\n      \"type\": \"string\",\n      \"title\": \"ControllerNamespace indicates the namespace in which the application controller is located\"\n    },\n    \"health\": {\n      \"$ref\": \"#/definitions/v1alpha1AppHealthStatus\"\n    },\n    \"history\": {\n      \"type\": \"array\",\n      \"title\": \"History contains information\
  \ about the application's sync history\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1RevisionHistory\"\n      }\n    },\n    \"observedAt\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"operationState\": {\n      \"$ref\": \"#/definitions/v1alpha1OperationState\"\n    },\n    \"reconciledAt\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"resourceHealthSource\": {\n      \"type\": \"string\",\n      \"title\": \"ResourceHealthSource indicates where the resource health status is stored: inline if not set or appTree\"\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"title\": \"Resources is a list of Kubernetes resources managed by this application\",\n      \"items\": {\n        \"$ref\": \"#/definitions/applicationv1alpha1ResourceStatus\"\n      }\n    },\n    \"sourceHydrator\": {\n      \"$ref\": \"#/definitions/v1alpha1SourceHydratorStatus\"\n    },\n    \"sourceType\": {\n      \"type\": \"string\",\n      \"title\": \"\
  SourceType specifies the type of this application\"\n    },\n    \"sourceTypes\": {\n      \"type\": \"array\",\n      \"title\": \"SourceTypes specifies the type of the sources included in the application\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"summary\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSummary\"\n    },\n    \"sync\": {\n      \"$ref\": \"#/definitions/v1alpha1SyncStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-status-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationStatus
---
