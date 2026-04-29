---
description: SyncOperation contains details about a sync operation.
layout: schema
name: v1alpha1SyncOperation
properties_list:
- description: ''
  name: autoHealAttemptsCount
  type: integer
- description: ''
  name: dryRun
  type: boolean
- description: ''
  name: manifests
  type: array
- description: ''
  name: prune
  type: boolean
- description: ''
  name: resources
  type: array
- description: Revision is the revision (Git) or chart version (Helm) which to sync the application to If omitted, will use the revision specified in app spec.
  name: revision
  type: string
- description: Revisions is the list of revision (Git) or chart version (Helm) which to sync each source in sources field for the application to If omitted, will use the revision specified in app spec.
  name: revisions
  type: array
- description: ''
  name: source
  type: object
- description: ''
  name: sources
  type: array
- description: ''
  name: syncOptions
  type: array
- description: ''
  name: syncStrategy
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-sync-operation-schema.json
slug: argo-cd-v1alpha1-sync-operation
source_filename: argo-cd-v1alpha1-sync-operation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-operation-schema.json\",\n  \"title\": \"v1alpha1SyncOperation\",\n  \"description\": \"SyncOperation contains details about a sync operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"autoHealAttemptsCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"SelfHealAttemptsCount contains the number of auto-heal attempts\"\n    },\n    \"dryRun\": {\n      \"type\": \"boolean\",\n      \"title\": \"DryRun specifies to perform a `kubectl apply --dry-run` without actually performing the sync\"\n    },\n    \"manifests\": {\n      \"type\": \"array\",\n      \"title\": \"Manifests is an optional field that overrides sync source with a local directory for development\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"prune\"\
  : {\n      \"type\": \"boolean\",\n      \"title\": \"Prune specifies to delete resources from the cluster that are no longer tracked in git\"\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"title\": \"Resources describes which resources shall be part of the sync\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1SyncOperationResource\"\n      }\n    },\n    \"revision\": {\n      \"description\": \"Revision is the revision (Git) or chart version (Helm) which to sync the application to\\nIf omitted, will use the revision specified in app spec.\",\n      \"type\": \"string\"\n    },\n    \"revisions\": {\n      \"description\": \"Revisions is the list of revision (Git) or chart version (Helm) which to sync each source in sources field for the application to\\nIf omitted, will use the revision specified in app spec.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"source\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSource\"\
  \n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"title\": \"Sources overrides the source definition set in the application.\\nThis is typically set in a Rollback operation and is nil during a Sync operation\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationSource\"\n      }\n    },\n    \"syncOptions\": {\n      \"type\": \"array\",\n      \"title\": \"SyncOptions provide per-sync sync-options, e.g. Validate=false\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"syncStrategy\": {\n      \"$ref\": \"#/definitions/v1alpha1SyncStrategy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-operation-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SyncOperation
---
