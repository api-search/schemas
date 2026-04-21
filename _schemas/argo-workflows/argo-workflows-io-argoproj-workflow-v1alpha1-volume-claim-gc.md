---
description: VolumeClaimGC describes how to delete volumes from completed Workflows
layout: schema
name: io.argoproj.workflow.v1alpha1.VolumeClaimGC
properties_list:
- description: Strategy is the strategy to use. One of "OnWorkflowCompletion", "OnWorkflowSuccess". Defaults to "OnWorkflowSuccess"
  name: strategy
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-volume-claim-gc-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-volume-claim-gc
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.VolumeClaimGC
---
