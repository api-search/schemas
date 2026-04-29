---
description: MutexStatus contains which objects hold mutex locks, and which objects this workflow is waiting on to release locks.
layout: schema
name: io.argoproj.workflow.v1alpha1.MutexStatus
properties_list:
- description: Holding is a list of mutexes and their respective objects that are held by mutex lock for this io.argoproj.workflow.v1alpha1.
  name: holding
  type: array
- description: Waiting is a list of mutexes and their respective objects this workflow is waiting for.
  name: waiting
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-mutex-status-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-mutex-status
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-mutex-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-mutex-status-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.MutexStatus\",\n  \"description\": \"MutexStatus contains which objects hold  mutex locks, and which objects this workflow is waiting on to release locks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"holding\": {\n      \"description\": \"Holding is a list of mutexes and their respective objects that are held by mutex lock for this io.argoproj.workflow.v1alpha1.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.MutexHolding\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"waiting\": {\n      \"description\": \"Waiting is a list of mutexes and their respective objects this workflow is waiting\
  \ for.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.MutexHolding\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-mutex-status-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.MutexStatus
---
