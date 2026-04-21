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
