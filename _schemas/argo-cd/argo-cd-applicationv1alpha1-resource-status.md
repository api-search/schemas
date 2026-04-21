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
