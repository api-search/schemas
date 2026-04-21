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
