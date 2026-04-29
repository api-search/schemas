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
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-pod-gc-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-pod-gc-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.PodGC\",\n  \"description\": \"PodGC describes how to delete completed pods as they complete\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deleteDelayDuration\": {\n      \"description\": \"DeleteDelayDuration specifies the duration before pods in the GC queue get deleted.\",\n      \"type\": \"string\"\n    },\n    \"labelSelector\": {\n      \"description\": \"LabelSelector is the label selector to check if the pods match the labels before being added to the pod GC queue.\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.LabelSelector\"\n    },\n    \"strategy\": {\n      \"description\": \"Strategy is the strategy to use. One of \\\"OnPodCompletion\\\", \\\"\
  OnPodSuccess\\\", \\\"OnWorkflowCompletion\\\", \\\"OnWorkflowSuccess\\\". If unset, does not delete Pods\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-pod-gc-schema.json
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
