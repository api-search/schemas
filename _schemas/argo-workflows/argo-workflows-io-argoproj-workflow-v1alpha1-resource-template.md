---
description: ResourceTemplate is a template subtype to manipulate kubernetes resources
layout: schema
name: io.argoproj.workflow.v1alpha1.ResourceTemplate
properties_list:
- description: 'Action is the action to perform to the resource. Must be one of: get, create, apply, delete, replace, patch'
  name: action
  type: string
- description: FailureCondition is a label selector expression which describes the conditions of the k8s resource in which the step was considered failed
  name: failureCondition
  type: string
- description: 'Flags is a set of additional options passed to kubectl before submitting a resource I.e. to disable resource validation: flags: [ "--validate=false" # disable resource validation ]'
  name: flags
  type: array
- description: Manifest contains the kubernetes manifest
  name: manifest
  type: string
- description: ManifestFrom is the source for a single kubernetes manifest
  name: manifestFrom
  type: object
- description: 'MergeStrategy is the strategy used to merge a patch. It defaults to "strategic" Must be one of: strategic, merge, json'
  name: mergeStrategy
  type: string
- description: SetOwnerReference sets the reference to the workflow on the OwnerReference of generated resource.
  name: setOwnerReference
  type: boolean
- description: SuccessCondition is a label selector expression which describes the conditions of the k8s resource in which it is acceptable to proceed to the following step
  name: successCondition
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-resource-template-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-resource-template
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ResourceTemplate
---
