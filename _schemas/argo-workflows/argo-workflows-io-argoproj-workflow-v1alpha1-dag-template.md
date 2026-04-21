---
description: DAGTemplate is a template subtype for directed acyclic graph templates
layout: schema
name: io.argoproj.workflow.v1alpha1.DAGTemplate
properties_list:
- description: 'This flag is for DAG logic. The DAG logic has a built-in "fail fast" feature to stop scheduling new steps, as soon as it detects that one of the DAG nodes is failed. Then it waits until all DAG nodes '
  name: failFast
  type: boolean
- description: Target are one or more names of targets to execute in a DAG
  name: target
  type: string
- description: Tasks are a list of DAG tasks MaxItems is an artificial limit to limit CEL validation costs - see note at top of file
  name: tasks
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-dag-template-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-dag-template
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.DAGTemplate
---
