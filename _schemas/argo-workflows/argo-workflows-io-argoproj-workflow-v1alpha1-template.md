---
description: Template is a reusable and composable unit of execution in a workflow
layout: schema
name: io.argoproj.workflow.v1alpha1.Template
properties_list:
- description: Optional duration in seconds relative to the StartTime that the pod may be active on a node before the system actively tries to terminate the pod; value must be positive integer This field is only app
  name: activeDeadlineSeconds
  type: object
- description: Affinity sets the pod's scheduling constraints Overrides the affinity set at the workflow level (if any)
  name: affinity
  type: object
- description: Annotations is a list of annotations to add to the template at runtime
  name: annotations
  type: object
- description: Location in which all files related to the step will be stored (logs, artifacts, etc...). Can be overridden by individual items in Outputs. If omitted, will use the default artifact repository locatio
  name: archiveLocation
  type: object
- description: AutomountServiceAccountToken indicates whether a service account token should be automatically mounted in pods. ServiceAccountName of ExecutorConfig must be specified if this value is false.
  name: automountServiceAccountToken
  type: boolean
- description: Container is the main container image to run in the pod
  name: container
  type: object
- description: ContainerSet groups multiple containers within a single pod.
  name: containerSet
  type: object
- description: Daemon will allow a workflow to proceed to the next step so long as the container reaches readiness
  name: daemon
  type: boolean
- description: DAG template subtype which runs a DAG
  name: dag
  type: object
- description: Data is a data template
  name: data
  type: object
- description: Executor holds configurations of the executor container.
  name: executor
  type: object
- description: FailFast, if specified, will fail this template if any of its child pods has failed. This is useful for when this template is expanded with `withItems`, etc.
  name: failFast
  type: boolean
- description: HostAliases is an optional list of hosts and IPs that will be injected into the pod spec
  name: hostAliases
  type: array
- description: HTTP makes a HTTP request
  name: http
  type: object
- description: InitContainers is a list of containers which run before the main container.
  name: initContainers
  type: array
- description: Inputs describe what inputs parameters and artifacts are supplied to this template
  name: inputs
  type: object
- description: Memoize allows templates to use outputs generated from already executed templates
  name: memoize
  type: object
- description: Metadata sets the pods's metadata, i.e. annotations and labels
  name: metadata
  type: object
- description: Metrics are a list of metrics emitted from this template
  name: metrics
  type: object
- description: Name is the name of the template
  name: name
  type: string
- description: NodeSelector is a selector to schedule this step of the workflow to be run on the selected node(s). Overrides the selector set at the workflow level.
  name: nodeSelector
  type: object
- description: Outputs describe the parameters and artifacts that this template produces
  name: outputs
  type: object
- description: Parallelism limits the max total parallel pods that can execute at the same time within the boundaries of this template invocation. If additional steps/dag templates are invoked, the pods created by t
  name: parallelism
  type: integer
- description: 'Plugin is a plugin template Note: the structure of a plugin template is free-form, so we need to have "x-kubernetes-preserve-unknown-fields: true" in the validation schema.'
  name: plugin
  type: object
- description: PodSpecPatch holds strategic merge patch to apply against the pod spec. Allows parameterization of container fields which are not strings (e.g. resource limits).
  name: podSpecPatch
  type: string
- description: PriorityClassName to apply to workflow pods.
  name: priorityClassName
  type: string
- description: Resource template subtype which can run k8s resources
  name: resource
  type: object
- description: RetryStrategy describes how to retry a template when it fails
  name: retryStrategy
  type: object
- description: If specified, the pod will be dispatched by specified scheduler. Or it will be dispatched by workflow scope scheduler if specified. If neither specified, the pod will be dispatched by default schedule
  name: schedulerName
  type: string
- description: Script runs a portion of code against an interpreter
  name: script
  type: object
- description: 'SecurityContext holds pod-level security attributes and common container settings. Optional: Defaults to empty. See type description for default values of each field.'
  name: securityContext
  type: object
- description: ServiceAccountName to apply to workflow pods
  name: serviceAccountName
  type: string
- description: Sidecars is a list of containers which run alongside the main container Sidecars are automatically killed when the main container completes
  name: sidecars
  type: array
- description: Steps define a series of sequential/parallel workflow steps
  name: steps
  type: array
- description: Suspend template subtype which can suspend a workflow when reaching the step
  name: suspend
  type: object
- description: Synchronization holds synchronization lock configuration for this template
  name: synchronization
  type: object
- description: Timeout allows to set the total node execution timeout duration counting from the node's start time. This duration also includes time in which the node spends in Pending state. This duration may not b
  name: timeout
  type: string
- description: Tolerations to apply to workflow pods.
  name: tolerations
  type: array
- description: Volumes is a list of volumes that can be mounted by containers in a template.
  name: volumes
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-template-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-template
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Template
---
