---
description: PodGC describes how to delete completed pods as they complete
layout: schema
name: io.argoproj.workflow.v1alpha1.PodGC
properties_list:
- description: DeleteDelayDuration specifies the duration before pods in the GC queue get deleted.
  name: deleteDelayDuration
  type: string
- description: LabelSelector is the label selector to check if the pods match the labels before being added to the pod GC queue.
  name: labelSelector
  type: object
- description: Strategy is the strategy to use. One of "OnPodCompletion", "OnPodSuccess", "OnWorkflowCompletion", "OnWorkflowSuccess". If unset, does not delete Pods
  name: strategy
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-pod-gc-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-pod-gc
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.PodGC
---
