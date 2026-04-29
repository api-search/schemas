---
description: WorkflowStatus contains overall status information about a workflow
layout: schema
name: io.argoproj.workflow.v1alpha1.WorkflowStatus
properties_list:
- description: ArtifactGCStatus maintains the status of Artifact Garbage Collection
  name: artifactGCStatus
  type: object
- description: ArtifactRepositoryRef is used to cache the repository to use so we do not need to determine it everytime we reconcile.
  name: artifactRepositoryRef
  type: object
- description: Compressed and base64 decoded Nodes map
  name: compressedNodes
  type: string
- description: Conditions is a list of conditions the Workflow may have
  name: conditions
  type: array
- description: EstimatedDuration in seconds.
  name: estimatedDuration
  type: integer
- description: Time at which this workflow completed
  name: finishedAt
  type: object
- description: A human readable message indicating details about why the workflow is in this condition.
  name: message
  type: string
- description: Nodes is a mapping between a node ID and the node's status.
  name: nodes
  type: object
- description: Whether on not node status has been offloaded to a database. If exists, then Nodes and CompressedNodes will be empty. This will actually be populated with a hash of the offloaded data.
  name: offloadNodeStatusVersion
  type: string
- description: Outputs captures output values and artifact locations produced by the workflow via global outputs
  name: outputs
  type: object
- description: PersistentVolumeClaims tracks all PVCs that were created as part of the io.argoproj.workflow.v1alpha1. The contents of this list are drained at the end of the workflow.
  name: persistentVolumeClaims
  type: array
- description: 'Phase a simple, high-level summary of where the workflow is in its lifecycle. Will be "" (Unknown), "Pending", or "Running" before the workflow is completed, and "Succeeded", "Failed" or "Error" once '
  name: phase
  type: string
- description: Progress to completion
  name: progress
  type: string
- description: ResourcesDuration is the total for the workflow
  name: resourcesDuration
  type: object
- description: Time at which this workflow started
  name: startedAt
  type: object
- description: StoredTemplates is a mapping between a template ref and the node's status.
  name: storedTemplates
  type: object
- description: StoredWorkflowSpec stores the WorkflowTemplate spec for future execution.
  name: storedWorkflowTemplateSpec
  type: object
- description: Synchronization stores the status of synchronization locks
  name: synchronization
  type: object
- description: TaskResultsCompletionStatus tracks task result completion status (mapped by node ID). Used to prevent premature archiving and garbage collection.
  name: taskResultsCompletionStatus
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-status-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-status
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-status-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.WorkflowStatus\",\n  \"description\": \"WorkflowStatus contains overall status information about a workflow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"artifactGCStatus\": {\n      \"description\": \"ArtifactGCStatus maintains the status of Artifact Garbage Collection\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ArtGCStatus\"\n    },\n    \"artifactRepositoryRef\": {\n      \"description\": \"ArtifactRepositoryRef is used to cache the repository to use so we do not need to determine it everytime we reconcile.\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ArtifactRepositoryRefStatus\"\n    },\n    \"compressedNodes\": {\n      \"description\"\
  : \"Compressed and base64 decoded Nodes map\",\n      \"type\": \"string\"\n    },\n    \"conditions\": {\n      \"description\": \"Conditions is a list of conditions the Workflow may have\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Condition\"\n      }\n    },\n    \"estimatedDuration\": {\n      \"description\": \"EstimatedDuration in seconds.\",\n      \"type\": \"integer\"\n    },\n    \"finishedAt\": {\n      \"description\": \"Time at which this workflow completed\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.Time\"\n    },\n    \"message\": {\n      \"description\": \"A human readable message indicating details about why the workflow is in this condition.\",\n      \"type\": \"string\"\n    },\n    \"nodes\": {\n      \"description\": \"Nodes is a mapping between a node ID and the node's status.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"\
  #/definitions/io.argoproj.workflow.v1alpha1.NodeStatus\"\n      }\n    },\n    \"offloadNodeStatusVersion\": {\n      \"description\": \"Whether on not node status has been offloaded to a database. If exists, then Nodes and CompressedNodes will be empty. This will actually be populated with a hash of the offloaded data.\",\n      \"type\": \"string\"\n    },\n    \"outputs\": {\n      \"description\": \"Outputs captures output values and artifact locations produced by the workflow via global outputs\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Outputs\"\n    },\n    \"persistentVolumeClaims\": {\n      \"description\": \"PersistentVolumeClaims tracks all PVCs that were created as part of the io.argoproj.workflow.v1alpha1. The contents of this list are drained at the end of the workflow.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.Volume\"\n      }\n    },\n    \"phase\": {\n      \"description\": \"Phase\
  \ a simple, high-level summary of where the workflow is in its lifecycle. Will be \\\"\\\" (Unknown), \\\"Pending\\\", or \\\"Running\\\" before the workflow is completed, and \\\"Succeeded\\\", \\\"Failed\\\" or \\\"Error\\\" once the workflow has completed.\",\n      \"type\": \"string\"\n    },\n    \"progress\": {\n      \"description\": \"Progress to completion\",\n      \"type\": \"string\"\n    },\n    \"resourcesDuration\": {\n      \"description\": \"ResourcesDuration is the total for the workflow\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      }\n    },\n    \"startedAt\": {\n      \"description\": \"Time at which this workflow started\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.Time\"\n    },\n    \"storedTemplates\": {\n      \"description\": \"StoredTemplates is a mapping between a template ref and the node's status.\",\n      \"type\": \"object\",\n      \"\
  additionalProperties\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Template\"\n      }\n    },\n    \"storedWorkflowTemplateSpec\": {\n      \"description\": \"StoredWorkflowSpec stores the WorkflowTemplate spec for future execution.\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.WorkflowSpec\"\n    },\n    \"synchronization\": {\n      \"description\": \"Synchronization stores the status of synchronization locks\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.SynchronizationStatus\"\n    },\n    \"taskResultsCompletionStatus\": {\n      \"description\": \"TaskResultsCompletionStatus tracks task result completion status (mapped by node ID). Used to prevent premature archiving and garbage collection.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"boolean\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-status-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.WorkflowStatus
---
