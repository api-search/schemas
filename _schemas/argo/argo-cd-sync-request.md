---
description: Request body for triggering an application sync operation.
layout: schema
name: SyncRequest
properties_list:
- description: Specific Git revision to sync to. Defaults to the current target revision.
  name: revision
  type: string
- description: Preview sync without applying changes.
  name: dryRun
  type: boolean
- description: Delete resources no longer defined in the source.
  name: prune
  type: boolean
- description: Sync strategy configuration.
  name: strategy
  type: object
- description: Specific resources to sync (partial sync).
  name: resources
  type: array
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-sync-request-schema.json
slug: argo-cd-sync-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-sync-request-schema.json\",\n  \"title\": \"SyncRequest\",\n  \"description\": \"Request body for triggering an application sync operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"revision\": {\n      \"type\": \"string\",\n      \"description\": \"Specific Git revision to sync to. Defaults to the current target revision.\"\n    },\n    \"dryRun\": {\n      \"type\": \"boolean\",\n      \"description\": \"Preview sync without applying changes.\"\n    },\n    \"prune\": {\n      \"type\": \"boolean\",\n      \"description\": \"Delete resources no longer defined in the source.\"\n    },\n    \"strategy\": {\n      \"type\": \"object\",\n      \"description\": \"Sync strategy configuration.\",\n      \"properties\": {\n        \"apply\": {\n          \"type\": \"object\",\n          \"description\"\
  : \"Use kubectl apply sync strategy.\",\n          \"properties\": {\n            \"force\": {\n              \"type\": \"boolean\",\n              \"description\": \"Force resource updates through delete and recreate.\"\n            }\n          }\n        },\n        \"hook\": {\n          \"type\": \"object\",\n          \"description\": \"Use hook-based sync strategy.\",\n          \"properties\": {\n            \"force\": {\n              \"type\": \"boolean\",\n              \"description\": \"Force resource updates.\"\n            }\n          }\n        }\n      }\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"Specific resources to sync (partial sync).\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"group\": {\n            \"type\": \"string\",\n            \"description\": \"Kubernetes API group.\"\n          },\n          \"kind\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"Resource kind.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Resource name.\"\n          },\n          \"namespace\": {\n            \"type\": \"string\",\n            \"description\": \"Resource namespace.\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-sync-request-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: SyncRequest
---
