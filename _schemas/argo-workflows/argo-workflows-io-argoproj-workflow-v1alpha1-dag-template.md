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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-dag-template-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.DAGTemplate\",\n  \"description\": \"DAGTemplate is a template subtype for directed acyclic graph templates\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"failFast\": {\n      \"description\": \"This flag is for DAG logic. The DAG logic has a built-in \\\"fail fast\\\" feature to stop scheduling new steps, as soon as it detects that one of the DAG nodes is failed. Then it waits until all DAG nodes are completed before failing the DAG itself. The FailFast flag default is true,  if set to false, it will allow a DAG to run all branches of the DAG to completion (either success or failure), regardless of the failed outcomes of branches in the DAG. More info and example about this feature\
  \ at https://github.com/argoproj/argo-workflows/issues/1442\",\n      \"type\": \"boolean\"\n    },\n    \"target\": {\n      \"description\": \"Target are one or more names of targets to execute in a DAG\",\n      \"type\": \"string\"\n    },\n    \"tasks\": {\n      \"description\": \"Tasks are a list of DAG tasks MaxItems is an artificial limit to limit CEL validation costs - see note at top of file\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.DAGTask\"\n      },\n      \"x-kubernetes-patch-merge-key\": \"name\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    }\n  },\n  \"required\": [\n    \"tasks\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-dag-template-schema.json
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
