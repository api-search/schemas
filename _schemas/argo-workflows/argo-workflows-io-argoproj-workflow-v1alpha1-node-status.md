---
description: NodeStatus contains status information about an individual node in the workflow
layout: schema
name: io.argoproj.workflow.v1alpha1.NodeStatus
properties_list:
- description: BoundaryID indicates the node ID of the associated template root node in which this node belongs to
  name: boundaryID
  type: string
- description: Children is a list of child node IDs
  name: children
  type: array
- description: Daemoned tracks whether or not this node was daemoned and need to be terminated
  name: daemoned
  type: boolean
- description: DisplayName is a human readable representation of the node. Unique within a template boundary
  name: displayName
  type: string
- description: EstimatedDuration in seconds.
  name: estimatedDuration
  type: integer
- description: FailedPodRestarts tracks the number of times the pod for this node was restarted due to infrastructure failures before the main container started.
  name: failedPodRestarts
  type: integer
- description: Time at which this node completed
  name: finishedAt
  type: object
- description: HostNodeName name of the Kubernetes node on which the Pod is running, if applicable
  name: hostNodeName
  type: string
- description: ID is a unique identifier of a node within the worklow It is implemented as a hash of the node name, which makes the ID deterministic
  name: id
  type: string
- description: Inputs captures input parameter values and artifact locations supplied to this template invocation
  name: inputs
  type: object
- description: MemoizationStatus holds information about cached nodes
  name: memoizationStatus
  type: object
- description: A human readable message indicating details about why the node is in this condition.
  name: message
  type: string
- description: Name is unique name in the node tree used to generate the node ID
  name: name
  type: string
- description: NodeFlag tracks some history of node. e.g.) hooked, retried, etc.
  name: nodeFlag
  type: object
- description: OutboundNodes tracks the node IDs which are considered "outbound" nodes to a template invocation. For every invocation of a template, there are nodes which we considered as "outbound". Essentially, th
  name: outboundNodes
  type: array
- description: Outputs captures output parameter values and artifact locations produced by this template invocation
  name: outputs
  type: object
- description: Phase a simple, high-level summary of where the node is in its lifecycle. Can be used as a state machine. Will be one of these values "Pending", "Running" before the node is completed, or "Succeeded",
  name: phase
  type: string
- description: PodIP captures the IP of the pod for daemoned steps
  name: podIP
  type: string
- description: Progress to completion
  name: progress
  type: string
- description: ResourcesDuration is indicative, but not accurate, resource duration. This is populated when the nodes completes.
  name: resourcesDuration
  type: object
- description: RestartingPodUID tracks the UID of the pod that is currently being restarted. This prevents duplicate restart attempts when the controller processes the same failed pod multiple times. Cleared when th
  name: restartingPodUID
  type: string
- description: Time at which this node started
  name: startedAt
  type: object
- description: SynchronizationStatus is the synchronization status of the node
  name: synchronizationStatus
  type: object
- description: TaskResultSynced is used to determine if the node's output has been received
  name: taskResultSynced
  type: boolean
- description: TemplateName is the template name which this node corresponds to. Not applicable to virtual nodes (e.g. Retry, StepGroup)
  name: templateName
  type: string
- description: TemplateRef is the reference to the template resource which this node corresponds to. Not applicable to virtual nodes (e.g. Retry, StepGroup)
  name: templateRef
  type: object
- description: TemplateScope is the template scope in which the template of this node was retrieved.
  name: templateScope
  type: string
- description: Type indicates type of node
  name: type
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-node-status-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-node-status
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-node-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-node-status-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.NodeStatus\",\n  \"description\": \"NodeStatus contains status information about an individual node in the workflow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"boundaryID\": {\n      \"description\": \"BoundaryID indicates the node ID of the associated template root node in which this node belongs to\",\n      \"type\": \"string\"\n    },\n    \"children\": {\n      \"description\": \"Children is a list of child node IDs\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"daemoned\": {\n      \"description\": \"Daemoned tracks whether or not this node was daemoned and need to be terminated\",\n      \"type\": \"boolean\"\n\
  \    },\n    \"displayName\": {\n      \"description\": \"DisplayName is a human readable representation of the node. Unique within a template boundary\",\n      \"type\": \"string\"\n    },\n    \"estimatedDuration\": {\n      \"description\": \"EstimatedDuration in seconds.\",\n      \"type\": \"integer\"\n    },\n    \"failedPodRestarts\": {\n      \"description\": \"FailedPodRestarts tracks the number of times the pod for this node was restarted due to infrastructure failures before the main container started.\",\n      \"type\": \"integer\"\n    },\n    \"finishedAt\": {\n      \"description\": \"Time at which this node completed\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.Time\"\n    },\n    \"hostNodeName\": {\n      \"description\": \"HostNodeName name of the Kubernetes node on which the Pod is running, if applicable\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"ID is a unique identifier of a node within the worklow\
  \ It is implemented as a hash of the node name, which makes the ID deterministic\",\n      \"type\": \"string\"\n    },\n    \"inputs\": {\n      \"description\": \"Inputs captures input parameter values and artifact locations supplied to this template invocation\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Inputs\"\n    },\n    \"memoizationStatus\": {\n      \"description\": \"MemoizationStatus holds information about cached nodes\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.MemoizationStatus\"\n    },\n    \"message\": {\n      \"description\": \"A human readable message indicating details about why the node is in this condition.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name is unique name in the node tree used to generate the node ID\",\n      \"type\": \"string\"\n    },\n    \"nodeFlag\": {\n      \"description\": \"NodeFlag tracks some history of node. e.g.) hooked, retried, etc.\",\n      \"$ref\"\
  : \"#/definitions/io.argoproj.workflow.v1alpha1.NodeFlag\"\n    },\n    \"outboundNodes\": {\n      \"description\": \"OutboundNodes tracks the node IDs which are considered \\\"outbound\\\" nodes to a template invocation. For every invocation of a template, there are nodes which we considered as \\\"outbound\\\". Essentially, these are last nodes in the execution sequence to run, before the template is considered completed. These nodes are then connected as parents to a following step.\\n\\nIn the case of single pod steps (i.e. container, script, resource templates), this list will be nil since the pod itself is already considered the \\\"outbound\\\" node. In the case of DAGs, outbound nodes are the \\\"target\\\" tasks (tasks with no children). In the case of steps, outbound nodes are all the containers involved in the last step group. NOTE: since templates are composable, the list of outbound nodes are carried upwards when a DAG/steps template invokes another DAG/steps template. In\
  \ other words, the outbound nodes of a template, will be a superset of the outbound nodes of its last children.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"outputs\": {\n      \"description\": \"Outputs captures output parameter values and artifact locations produced by this template invocation\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Outputs\"\n    },\n    \"phase\": {\n      \"description\": \"Phase a simple, high-level summary of where the node is in its lifecycle. Can be used as a state machine. Will be one of these values \\\"Pending\\\", \\\"Running\\\" before the node is completed, or \\\"Succeeded\\\", \\\"Skipped\\\", \\\"Failed\\\", \\\"Error\\\", or \\\"Omitted\\\" as a final state.\",\n      \"type\": \"string\"\n    },\n    \"podIP\": {\n      \"description\": \"PodIP captures the IP of the pod for daemoned steps\",\n      \"type\": \"string\"\n    },\n    \"progress\": {\n      \"description\"\
  : \"Progress to completion\",\n      \"type\": \"string\"\n    },\n    \"resourcesDuration\": {\n      \"description\": \"ResourcesDuration is indicative, but not accurate, resource duration. This is populated when the nodes completes.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      }\n    },\n    \"restartingPodUID\": {\n      \"description\": \"RestartingPodUID tracks the UID of the pod that is currently being restarted. This prevents duplicate restart attempts when the controller processes the same failed pod multiple times. Cleared when the replacement pod starts running.\",\n      \"type\": \"string\"\n    },\n    \"startedAt\": {\n      \"description\": \"Time at which this node started\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.Time\"\n    },\n    \"synchronizationStatus\": {\n      \"description\": \"SynchronizationStatus is the synchronization status of the node\"\
  ,\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.NodeSynchronizationStatus\"\n    },\n    \"taskResultSynced\": {\n      \"description\": \"TaskResultSynced is used to determine if the node's output has been received\",\n      \"type\": \"boolean\"\n    },\n    \"templateName\": {\n      \"description\": \"TemplateName is the template name which this node corresponds to. Not applicable to virtual nodes (e.g. Retry, StepGroup)\",\n      \"type\": \"string\"\n    },\n    \"templateRef\": {\n      \"description\": \"TemplateRef is the reference to the template resource which this node corresponds to. Not applicable to virtual nodes (e.g. Retry, StepGroup)\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.TemplateRef\"\n    },\n    \"templateScope\": {\n      \"description\": \"TemplateScope is the template scope in which the template of this node was retrieved.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type indicates\
  \ type of node\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-node-status-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.NodeStatus
---
