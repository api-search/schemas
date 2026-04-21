---
description: WorkflowSpec is the specification of a Workflow.
layout: schema
name: io.argoproj.workflow.v1alpha1.WorkflowSpec
properties_list:
- description: Optional duration in seconds relative to the workflow start time which the workflow is allowed to run before the controller terminates the io.argoproj.workflow.v1alpha1. A value of zero is used to ter
  name: activeDeadlineSeconds
  type: integer
- description: Affinity sets the scheduling constraints for all pods in the io.argoproj.workflow.v1alpha1. Can be overridden by an affinity specified in the template
  name: affinity
  type: object
- description: ArchiveLogs indicates if the container logs should be archived
  name: archiveLogs
  type: boolean
- description: Arguments contain the parameters and artifacts sent to the workflow entrypoint Parameters are referencable globally using the 'workflow' variable prefix. e.g. {{io.argoproj.workflow.v1alpha1.parameter
  name: arguments
  type: object
- description: ArtifactGC describes the strategy to use when deleting artifacts from completed or deleted workflows (applies to all output Artifacts unless Artifact.ArtifactGC is specified, which overrides this)
  name: artifactGC
  type: object
- description: ArtifactRepositoryRef specifies the configMap name and key containing the artifact repository config.
  name: artifactRepositoryRef
  type: object
- description: AutomountServiceAccountToken indicates whether a service account token should be automatically mounted in pods. ServiceAccountName of ExecutorConfig must be specified if this value is false.
  name: automountServiceAccountToken
  type: boolean
- description: PodDNSConfig defines the DNS parameters of a pod in addition to those generated from DNSPolicy.
  name: dnsConfig
  type: object
- description: Set DNS policy for workflow pods. Defaults to "ClusterFirst". Valid values are 'ClusterFirstWithHostNet', 'ClusterFirst', 'Default' or 'None'. DNS parameters given in DNSConfig will be merged with the
  name: dnsPolicy
  type: string
- description: Entrypoint is a template reference to the starting point of the io.argoproj.workflow.v1alpha1.
  name: entrypoint
  type: string
- description: Executor holds configurations of executor containers of the io.argoproj.workflow.v1alpha1.
  name: executor
  type: object
- description: Hooks holds the lifecycle hook which is invoked at lifecycle of step, irrespective of the success, failure, or error status of the primary step
  name: hooks
  type: object
- description: ''
  name: hostAliases
  type: array
- description: Host networking requested for this workflow pod. Default to false.
  name: hostNetwork
  type: boolean
- description: ImagePullSecrets is a list of references to secrets in the same namespace to use for pulling any images in pods that reference this ServiceAccount. ImagePullSecrets are distinct from Secrets because S
  name: imagePullSecrets
  type: array
- description: Metrics are a list of metrics emitted from this Workflow
  name: metrics
  type: object
- description: NodeSelector is a selector which will result in all pods of the workflow to be scheduled on the selected node(s). This is able to be overridden by a nodeSelector specified in the template.
  name: nodeSelector
  type: object
- description: OnExit is a template reference which is invoked at the end of the workflow, irrespective of the success, failure, or error of the primary io.argoproj.workflow.v1alpha1.
  name: onExit
  type: string
- description: Parallelism limits the max total parallel pods that can execute at the same time in a workflow
  name: parallelism
  type: integer
- description: 'PodDisruptionBudget holds the number of concurrent disruptions that you allow for Workflow''s Pods. Controller will automatically add the selector with workflow name, if selector is empty. Optional: De'
  name: podDisruptionBudget
  type: object
- description: PodGC describes the strategy to use when deleting completed pods
  name: podGC
  type: object
- description: PodMetadata defines additional metadata that should be applied to workflow pods
  name: podMetadata
  type: object
- description: PriorityClassName to apply to workflow pods.
  name: podPriorityClassName
  type: string
- description: PodSpecPatch holds strategic merge patch to apply against the pod spec. Allows parameterization of container fields which are not strings (e.g. resource limits).
  name: podSpecPatch
  type: string
- description: Priority is used if controller is configured to process limited number of workflows in parallel. Workflows with higher priority are processed first.
  name: priority
  type: integer
- description: RetryStrategy for all templates in the io.argoproj.workflow.v1alpha1.
  name: retryStrategy
  type: object
- description: Set scheduler name for all pods. Will be overridden if container/script template's scheduler name is set. Default scheduler will be used if neither specified.
  name: schedulerName
  type: string
- description: 'SecurityContext holds pod-level security attributes and common container settings. Optional: Defaults to empty. See type description for default values of each field.'
  name: securityContext
  type: object
- description: ServiceAccountName is the name of the ServiceAccount to run all pods of the workflow as.
  name: serviceAccountName
  type: string
- description: Shutdown will shutdown the workflow according to its ShutdownStrategy
  name: shutdown
  type: string
- description: Suspend will suspend the workflow and prevent execution of any future steps in the workflow
  name: suspend
  type: boolean
- description: Synchronization holds synchronization lock configuration for this Workflow
  name: synchronization
  type: object
- description: TemplateDefaults holds default template values that will apply to all templates in the Workflow, unless overridden on the template-level
  name: templateDefaults
  type: object
- description: Templates is a list of workflow templates used in a workflow MaxItems is an artificial limit to limit CEL validation costs - see note at top of file
  name: templates
  type: array
- description: Tolerations to apply to workflow pods.
  name: tolerations
  type: array
- description: TTLStrategy limits the lifetime of a Workflow that has finished execution depending on if it Succeeded or Failed. If this struct is set, once the Workflow finishes, it will be deleted after the time t
  name: ttlStrategy
  type: object
- description: VolumeClaimGC describes the strategy to use when deleting volumes from completed workflows
  name: volumeClaimGC
  type: object
- description: VolumeClaimTemplates is a list of claims that containers are allowed to reference. The Workflow controller will create the claims at the beginning of the workflow and delete the claims upon completion
  name: volumeClaimTemplates
  type: array
- description: Volumes is a list of volumes that can be mounted by containers in a io.argoproj.workflow.v1alpha1.
  name: volumes
  type: array
- description: WorkflowMetadata contains some metadata of the workflow to refer to
  name: workflowMetadata
  type: object
- description: WorkflowTemplateRef holds a reference to a WorkflowTemplate for execution
  name: workflowTemplateRef
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-spec-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-spec
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.WorkflowSpec
---
