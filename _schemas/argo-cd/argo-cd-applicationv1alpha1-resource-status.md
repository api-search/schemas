---
description: ResourceStatus holds the current synchronization and health status of a Kubernetes resource.
layout: schema
name: applicationv1alpha1ResourceStatus
properties_list:
- description: Group represents the API group of the resource (e.g., "apps" for Deployments).
  name: group
  type: string
- description: ''
  name: health
  type: object
- description: Hook is true if the resource is used as a lifecycle hook in an Argo CD application.
  name: hook
  type: boolean
- description: Kind specifies the type of the resource (e.g., "Deployment", "Service").
  name: kind
  type: string
- description: Name is the unique name of the resource within the namespace.
  name: name
  type: string
- description: Namespace defines the Kubernetes namespace where the resource is located.
  name: namespace
  type: string
- description: RequiresDeletionConfirmation is true if the resource requires explicit user confirmation before deletion.
  name: requiresDeletionConfirmation
  type: boolean
- description: RequiresPruning is true if the resource needs to be pruned (deleted) as part of synchronization.
  name: requiresPruning
  type: boolean
- description: Status represents the synchronization state of the resource (e.g., Synced, OutOfSync).
  name: status
  type: string
- description: SyncWave determines the order in which resources are applied during a sync operation. Lower values are applied first.
  name: syncWave
  type: integer
- description: Version indicates the API version of the resource (e.g., "v1", "v1beta1").
  name: version
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-applicationv1alpha1-resource-status-schema.json
slug: argo-cd-applicationv1alpha1-resource-status
source_filename: argo-cd-applicationv1alpha1-resource-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-applicationv1alpha1-resource-status-schema.json\",\n  \"title\": \"applicationv1alpha1ResourceStatus\",\n  \"description\": \"ResourceStatus holds the current synchronization and health status of a Kubernetes resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"group\": {\n      \"description\": \"Group represents the API group of the resource (e.g., \\\"apps\\\" for Deployments).\",\n      \"type\": \"string\"\n    },\n    \"health\": {\n      \"$ref\": \"#/definitions/v1alpha1HealthStatus\"\n    },\n    \"hook\": {\n      \"description\": \"Hook is true if the resource is used as a lifecycle hook in an Argo CD application.\",\n      \"type\": \"boolean\"\n    },\n    \"kind\": {\n      \"description\": \"Kind specifies the type of the resource (e.g., \\\"Deployment\\\", \\\"Service\\\").\"\
  ,\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name is the unique name of the resource within the namespace.\",\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"description\": \"Namespace defines the Kubernetes namespace where the resource is located.\",\n      \"type\": \"string\"\n    },\n    \"requiresDeletionConfirmation\": {\n      \"description\": \"RequiresDeletionConfirmation is true if the resource requires explicit user confirmation before deletion.\",\n      \"type\": \"boolean\"\n    },\n    \"requiresPruning\": {\n      \"description\": \"RequiresPruning is true if the resource needs to be pruned (deleted) as part of synchronization.\",\n      \"type\": \"boolean\"\n    },\n    \"status\": {\n      \"description\": \"Status represents the synchronization state of the resource (e.g., Synced, OutOfSync).\",\n      \"type\": \"string\"\n    },\n    \"syncWave\": {\n      \"description\": \"SyncWave determines the order in which\
  \ resources are applied during a sync operation.\\nLower values are applied first.\",\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"version\": {\n      \"description\": \"Version indicates the API version of the resource (e.g., \\\"v1\\\", \\\"v1beta1\\\").\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-applicationv1alpha1-resource-status-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: applicationv1alpha1ResourceStatus
---
