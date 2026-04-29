---
description: v1alpha1ApplicationSetApplicationStatus schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSetApplicationStatus
properties_list:
- description: ''
  name: application
  type: string
- description: ''
  name: lastTransitionTime
  type: object
- description: ''
  name: message
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: step
  type: string
- description: TargetRevision tracks the desired revisions the Application should be synced to.
  name: targetrevisions
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-application-status-schema.json
slug: argo-cd-v1alpha1-application-set-application-status
source_filename: argo-cd-v1alpha1-application-set-application-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-application-status-schema.json\",\n  \"title\": \"v1alpha1ApplicationSetApplicationStatus\",\n  \"description\": \"v1alpha1ApplicationSetApplicationStatus schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"type\": \"string\",\n      \"title\": \"Application contains the name of the Application resource\"\n    },\n    \"lastTransitionTime\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"title\": \"Message contains human-readable message indicating details about the status\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"title\": \"Status contains the AppSet's perceived status of the managed Application resource\"\n    },\n    \"step\": {\n    \
  \  \"type\": \"string\",\n      \"title\": \"Step tracks which step this Application should be updated in\"\n    },\n    \"targetrevisions\": {\n      \"description\": \"TargetRevision tracks the desired revisions the Application should be synced to.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-application-status-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetApplicationStatus
---
