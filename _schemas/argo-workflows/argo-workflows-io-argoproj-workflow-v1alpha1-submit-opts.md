---
description: SubmitOpts are workflow submission options
layout: schema
name: io.argoproj.workflow.v1alpha1.SubmitOpts
properties_list:
- description: Annotations adds to metadata.labels
  name: annotations
  type: string
- description: DryRun validates the workflow on the client-side without creating it. This option is not supported in API
  name: dryRun
  type: boolean
- description: Entrypoint overrides spec.entrypoint
  name: entryPoint
  type: string
- description: GenerateName overrides metadata.generateName
  name: generateName
  type: string
- description: Labels adds to metadata.labels
  name: labels
  type: string
- description: Name overrides metadata.name
  name: name
  type: string
- description: OwnerReference creates a metadata.ownerReference
  name: ownerReference
  type: object
- description: Parameters passes input parameters to workflow
  name: parameters
  type: array
- description: Set the podPriorityClassName of the workflow
  name: podPriorityClassName
  type: string
- description: Priority is used if controller is configured to process limited number of workflows in parallel, higher priority workflows are processed first.
  name: priority
  type: integer
- description: ServerDryRun validates the workflow on the server-side without creating it
  name: serverDryRun
  type: boolean
- description: ServiceAccount runs all pods in the workflow using specified ServiceAccount.
  name: serviceAccount
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-submit-opts-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-submit-opts
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.SubmitOpts
---
