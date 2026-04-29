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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-spec-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.WorkflowSpec\",\n  \"description\": \"WorkflowSpec is the specification of a Workflow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activeDeadlineSeconds\": {\n      \"description\": \"Optional duration in seconds relative to the workflow start time which the workflow is allowed to run before the controller terminates the io.argoproj.workflow.v1alpha1. A value of zero is used to terminate a Running workflow\",\n      \"type\": \"integer\"\n    },\n    \"affinity\": {\n      \"description\": \"Affinity sets the scheduling constraints for all pods in the io.argoproj.workflow.v1alpha1. Can be overridden by an affinity specified in the template\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.Affinity\"\
  \n    },\n    \"archiveLogs\": {\n      \"description\": \"ArchiveLogs indicates if the container logs should be archived\",\n      \"type\": \"boolean\"\n    },\n    \"arguments\": {\n      \"description\": \"Arguments contain the parameters and artifacts sent to the workflow entrypoint Parameters are referencable globally using the 'workflow' variable prefix. e.g. {{io.argoproj.workflow.v1alpha1.parameters.myparam}}\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Arguments\"\n    },\n    \"artifactGC\": {\n      \"description\": \"ArtifactGC describes the strategy to use when deleting artifacts from completed or deleted workflows (applies to all output Artifacts unless Artifact.ArtifactGC is specified, which overrides this)\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.WorkflowLevelArtifactGC\"\n    },\n    \"artifactRepositoryRef\": {\n      \"description\": \"ArtifactRepositoryRef specifies the configMap name and key containing the artifact repository\
  \ config.\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ArtifactRepositoryRef\"\n    },\n    \"automountServiceAccountToken\": {\n      \"description\": \"AutomountServiceAccountToken indicates whether a service account token should be automatically mounted in pods. ServiceAccountName of ExecutorConfig must be specified if this value is false.\",\n      \"type\": \"boolean\"\n    },\n    \"dnsConfig\": {\n      \"description\": \"PodDNSConfig defines the DNS parameters of a pod in addition to those generated from DNSPolicy.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.PodDNSConfig\"\n    },\n    \"dnsPolicy\": {\n      \"description\": \"Set DNS policy for workflow pods. Defaults to \\\"ClusterFirst\\\". Valid values are 'ClusterFirstWithHostNet', 'ClusterFirst', 'Default' or 'None'. DNS parameters given in DNSConfig will be merged with the policy selected with DNSPolicy. To have DNS options set along with hostNetwork, you have to specify DNS policy explicitly\
  \ to 'ClusterFirstWithHostNet'.\",\n      \"type\": \"string\"\n    },\n    \"entrypoint\": {\n      \"description\": \"Entrypoint is a template reference to the starting point of the io.argoproj.workflow.v1alpha1.\",\n      \"type\": \"string\"\n    },\n    \"executor\": {\n      \"description\": \"Executor holds configurations of executor containers of the io.argoproj.workflow.v1alpha1.\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ExecutorConfig\"\n    },\n    \"hooks\": {\n      \"description\": \"Hooks holds the lifecycle hook which is invoked at lifecycle of step, irrespective of the success, failure, or error status of the primary step\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.LifecycleHook\"\n      }\n    },\n    \"hostAliases\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.HostAlias\"\n      },\n      \"x-kubernetes-patch-merge-key\"\
  : \"ip\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    },\n    \"hostNetwork\": {\n      \"description\": \"Host networking requested for this workflow pod. Default to false.\",\n      \"type\": \"boolean\"\n    },\n    \"imagePullSecrets\": {\n      \"description\": \"ImagePullSecrets is a list of references to secrets in the same namespace to use for pulling any images in pods that reference this ServiceAccount. ImagePullSecrets are distinct from Secrets because Secrets can be mounted in the pod, but ImagePullSecrets are only accessed by the kubelet. More info: https://kubernetes.io/docs/concepts/containers/images/#specifying-imagepullsecrets-on-a-pod\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.LocalObjectReference\"\n      },\n      \"x-kubernetes-patch-merge-key\": \"name\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    },\n    \"metrics\": {\n      \"description\": \"Metrics are a list of metrics emitted\
  \ from this Workflow\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Metrics\"\n    },\n    \"nodeSelector\": {\n      \"description\": \"NodeSelector is a selector which will result in all pods of the workflow to be scheduled on the selected node(s). This is able to be overridden by a nodeSelector specified in the template.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"onExit\": {\n      \"description\": \"OnExit is a template reference which is invoked at the end of the workflow, irrespective of the success, failure, or error of the primary io.argoproj.workflow.v1alpha1.\",\n      \"type\": \"string\"\n    },\n    \"parallelism\": {\n      \"description\": \"Parallelism limits the max total parallel pods that can execute at the same time in a workflow\",\n      \"type\": \"integer\"\n    },\n    \"podDisruptionBudget\": {\n      \"description\": \"PodDisruptionBudget holds the number of concurrent\
  \ disruptions that you allow for Workflow's Pods. Controller will automatically add the selector with workflow name, if selector is empty. Optional: Defaults to empty.\",\n      \"$ref\": \"#/definitions/io.k8s.api.policy.v1.PodDisruptionBudgetSpec\"\n    },\n    \"podGC\": {\n      \"description\": \"PodGC describes the strategy to use when deleting completed pods\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.PodGC\"\n    },\n    \"podMetadata\": {\n      \"description\": \"PodMetadata defines additional metadata that should be applied to workflow pods\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Metadata\"\n    },\n    \"podPriorityClassName\": {\n      \"description\": \"PriorityClassName to apply to workflow pods.\",\n      \"type\": \"string\"\n    },\n    \"podSpecPatch\": {\n      \"description\": \"PodSpecPatch holds strategic merge patch to apply against the pod spec. Allows parameterization of container fields which are not strings (e.g.\
  \ resource limits).\",\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"description\": \"Priority is used if controller is configured to process limited number of workflows in parallel. Workflows with higher priority are processed first.\",\n      \"type\": \"integer\"\n    },\n    \"retryStrategy\": {\n      \"description\": \"RetryStrategy for all templates in the io.argoproj.workflow.v1alpha1.\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.RetryStrategy\"\n    },\n    \"schedulerName\": {\n      \"description\": \"Set scheduler name for all pods. Will be overridden if container/script template's scheduler name is set. Default scheduler will be used if neither specified.\",\n      \"type\": \"string\"\n    },\n    \"securityContext\": {\n      \"description\": \"SecurityContext holds pod-level security attributes and common container settings. Optional: Defaults to empty.  See type description for default values of each field.\",\n      \"$ref\": \"\
  #/definitions/io.k8s.api.core.v1.PodSecurityContext\"\n    },\n    \"serviceAccountName\": {\n      \"description\": \"ServiceAccountName is the name of the ServiceAccount to run all pods of the workflow as.\",\n      \"type\": \"string\"\n    },\n    \"shutdown\": {\n      \"description\": \"Shutdown will shutdown the workflow according to its ShutdownStrategy\",\n      \"type\": \"string\"\n    },\n    \"suspend\": {\n      \"description\": \"Suspend will suspend the workflow and prevent execution of any future steps in the workflow\",\n      \"type\": \"boolean\"\n    },\n    \"synchronization\": {\n      \"description\": \"Synchronization holds synchronization lock configuration for this Workflow\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Synchronization\"\n    },\n    \"templateDefaults\": {\n      \"description\": \"TemplateDefaults holds default template values that will apply to all templates in the Workflow, unless overridden on the template-level\",\n \
  \     \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Template\"\n    },\n    \"templates\": {\n      \"description\": \"Templates is a list of workflow templates used in a workflow MaxItems is an artificial limit to limit CEL validation costs - see note at top of file\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Template\"\n      },\n      \"x-kubernetes-patch-merge-key\": \"name\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    },\n    \"tolerations\": {\n      \"description\": \"Tolerations to apply to workflow pods.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.Toleration\"\n      },\n      \"x-kubernetes-patch-merge-key\": \"key\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    },\n    \"ttlStrategy\": {\n      \"description\": \"TTLStrategy limits the lifetime of a Workflow that has finished execution depending on if it Succeeded\
  \ or Failed. If this struct is set, once the Workflow finishes, it will be deleted after the time to live expires. If this field is unset, the controller config map will hold the default values.\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.TTLStrategy\"\n    },\n    \"volumeClaimGC\": {\n      \"description\": \"VolumeClaimGC describes the strategy to use when deleting volumes from completed workflows\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.VolumeClaimGC\"\n    },\n    \"volumeClaimTemplates\": {\n      \"description\": \"VolumeClaimTemplates is a list of claims that containers are allowed to reference. The Workflow controller will create the claims at the beginning of the workflow and delete the claims upon completion of the workflow\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.PersistentVolumeClaim\"\n      }\n    },\n    \"volumes\": {\n      \"description\": \"Volumes is a list\
  \ of volumes that can be mounted by containers in a io.argoproj.workflow.v1alpha1.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.Volume\"\n      },\n      \"x-kubernetes-patch-merge-key\": \"name\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    },\n    \"workflowMetadata\": {\n      \"description\": \"WorkflowMetadata contains some metadata of the workflow to refer to\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.WorkflowMetadata\"\n    },\n    \"workflowTemplateRef\": {\n      \"description\": \"WorkflowTemplateRef holds a reference to a WorkflowTemplate for execution\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.WorkflowTemplateRef\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-spec-schema.json
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
