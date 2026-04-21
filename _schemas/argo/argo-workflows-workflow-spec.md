---
description: Specification of a workflow
layout: schema
name: WorkflowSpec
properties_list:
- description: The name of the entrypoint template
  name: entrypoint
  type: string
- description: ''
  name: arguments
  type: object
- description: List of workflow templates
  name: templates
  type: array
- description: Service account to run workflow pods
  name: serviceAccountName
  type: string
- description: Volumes available to workflow steps
  name: volumes
  type: array
- description: Duration in seconds before workflow times out
  name: activeDeadlineSeconds
  type: integer
- description: ''
  name: nodeSelector
  type: object
- description: ''
  name: tolerations
  type: array
- description: Maximum number of parallel running pods
  name: parallelism
  type: integer
- description: Strategy for cleaning up completed workflows
  name: ttlStrategy
  type: object
- description: Strategy for garbage collecting completed pods
  name: podGC
  type: object
- description: Reference to a WorkflowTemplate
  name: workflowTemplateRef
  type: object
- description: Whether to archive workflow logs
  name: archiveLogs
  type: boolean
- description: Lifecycle hooks for the workflow
  name: hooks
  type: object
- description: Template to execute on workflow exit
  name: onExit
  type: string
- description: ''
  name: retryStrategy
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-workflow-spec-schema.json
slug: argo-workflows-workflow-spec
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: WorkflowSpec
---
