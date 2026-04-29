---
description: Observed state and operational status of an Argo CD application.
layout: schema
name: ApplicationStatus
properties_list:
- description: Current sync status.
  name: sync
  type: object
- description: Current health status.
  name: health
  type: object
- description: State of the current or most recent operation.
  name: operationState
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-application-status-schema.json
slug: argo-cd-application-status
source_filename: argo-cd-application-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-application-status-schema.json\",\n  \"title\": \"ApplicationStatus\",\n  \"description\": \"Observed state and operational status of an Argo CD application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sync\": {\n      \"type\": \"object\",\n      \"description\": \"Current sync status.\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Sync status (Synced, OutOfSync, Unknown).\",\n          \"enum\": [\n            \"Synced\",\n            \"OutOfSync\",\n            \"Unknown\"\n          ]\n        },\n        \"revision\": {\n          \"type\": \"string\",\n          \"description\": \"Deployed Git revision (commit SHA).\"\n        }\n      }\n    },\n    \"health\": {\n      \"type\": \"object\",\n      \"description\": \"Current\
  \ health status.\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Health status (Healthy, Progressing, Degraded, Suspended, Missing, Unknown).\",\n          \"enum\": [\n            \"Healthy\",\n            \"Progressing\",\n            \"Degraded\",\n            \"Suspended\",\n            \"Missing\",\n            \"Unknown\"\n          ]\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable health status message.\"\n        }\n      }\n    },\n    \"operationState\": {\n      \"type\": \"object\",\n      \"description\": \"State of the current or most recent operation.\",\n      \"properties\": {\n        \"phase\": {\n          \"type\": \"string\",\n          \"description\": \"Operation phase (Running, Failed, Succeeded, Error, Terminating).\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable\
  \ operation status message.\"\n        },\n        \"startedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the operation started.\"\n        },\n        \"finishedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the operation finished.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-application-status-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: ApplicationStatus
---
