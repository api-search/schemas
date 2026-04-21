---
description: ArtifactGC describes how to delete artifacts from completed Workflows - this is embedded into the WorkflowLevelArtifactGC, and also used for individual Artifacts to override that as needed
layout: schema
name: io.argoproj.workflow.v1alpha1.ArtifactGC
properties_list:
- description: PodMetadata is an optional field for specifying the Labels and Annotations that should be assigned to the Pod doing the deletion
  name: podMetadata
  type: object
- description: ServiceAccountName is an optional field for specifying the Service Account that should be assigned to the Pod doing the deletion
  name: serviceAccountName
  type: string
- description: Strategy is the strategy to use.
  name: strategy
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-gc-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-artifact-gc
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ArtifactGC
---
