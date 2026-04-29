---
description: Mutex holds Mutex configuration
layout: schema
name: io.argoproj.workflow.v1alpha1.Mutex
properties_list:
- description: Database specifies this is database controlled if this is set true
  name: database
  type: boolean
- description: name of the mutex
  name: name
  type: string
- description: 'Namespace is the namespace of the mutex, default: [namespace of workflow]'
  name: namespace
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-mutex-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-mutex
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-mutex-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Mutex\",\n  \"description\": \"Mutex holds Mutex configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"database\": {\n      \"description\": \"Database specifies this is database controlled if this is set true\",\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"description\": \"name of the mutex\",\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"description\": \"Namespace is the namespace of the mutex, default: [namespace of workflow]\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-mutex-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Mutex
---
