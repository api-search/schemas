---
description: MutexHolding describes the mutex and the object which is holding it.
layout: schema
name: io.argoproj.workflow.v1alpha1.MutexHolding
properties_list:
- description: 'Holder is a reference to the object which holds the Mutex. Holding Scenario: 1. Current workflow''s NodeID which is holding the lock. e.g: ${NodeID} Waiting Scenario: 1. Current workflow or other workf'
  name: holder
  type: string
- description: 'Reference for the mutex e.g: ${namespace}/mutex/${mutexName}'
  name: mutex
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-mutex-holding-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-mutex-holding
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-mutex-holding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-mutex-holding-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.MutexHolding\",\n  \"description\": \"MutexHolding describes the mutex and the object which is holding it.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"holder\": {\n      \"description\": \"Holder is a reference to the object which holds the Mutex. Holding Scenario:\\n  1. Current workflow's NodeID which is holding the lock.\\n     e.g: ${NodeID}\\nWaiting Scenario:\\n  1. Current workflow or other workflow NodeID which is holding the lock.\\n     e.g: ${WorkflowName}/${NodeID}\",\n      \"type\": \"string\"\n    },\n    \"mutex\": {\n      \"description\": \"Reference for the mutex e.g: ${namespace}/mutex/${mutexName}\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-mutex-holding-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.MutexHolding
---
