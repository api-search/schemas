---
description: WorkflowLevelArtifactGC describes how to delete artifacts from completed Workflows - this spec is used on the Workflow level
layout: schema
name: io.argoproj.workflow.v1alpha1.WorkflowLevelArtifactGC
properties_list:
- description: 'ForceFinalizerRemoval: if set to true, the finalizer will be removed in the case that Artifact GC fails'
  name: forceFinalizerRemoval
  type: boolean
- description: PodMetadata is an optional field for specifying the Labels and Annotations that should be assigned to the Pod doing the deletion
  name: podMetadata
  type: object
- description: PodSpecPatch holds strategic merge patch to apply against the artgc pod spec.
  name: podSpecPatch
  type: string
- description: ServiceAccountName is an optional field for specifying the Service Account that should be assigned to the Pod doing the deletion
  name: serviceAccountName
  type: string
- description: Strategy is the strategy to use.
  name: strategy
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-level-artifact-gc-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-level-artifact-gc
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-level-artifact-gc-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-level-artifact-gc-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.WorkflowLevelArtifactGC\",\n  \"description\": \"WorkflowLevelArtifactGC describes how to delete artifacts from completed Workflows - this spec is used on the Workflow level\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"forceFinalizerRemoval\": {\n      \"description\": \"ForceFinalizerRemoval: if set to true, the finalizer will be removed in the case that Artifact GC fails\",\n      \"type\": \"boolean\"\n    },\n    \"podMetadata\": {\n      \"description\": \"PodMetadata is an optional field for specifying the Labels and Annotations that should be assigned to the Pod doing the deletion\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Metadata\"\
  \n    },\n    \"podSpecPatch\": {\n      \"description\": \"PodSpecPatch holds strategic merge patch to apply against the artgc pod spec.\",\n      \"type\": \"string\"\n    },\n    \"serviceAccountName\": {\n      \"description\": \"ServiceAccountName is an optional field for specifying the Service Account that should be assigned to the Pod doing the deletion\",\n      \"type\": \"string\"\n    },\n    \"strategy\": {\n      \"description\": \"Strategy is the strategy to use.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-level-artifact-gc-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.WorkflowLevelArtifactGC
---
