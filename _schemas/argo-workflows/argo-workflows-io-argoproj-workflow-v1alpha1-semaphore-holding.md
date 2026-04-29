---
description: io.argoproj.workflow.v1alpha1.SemaphoreHolding schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.SemaphoreHolding
properties_list:
- description: Holders stores the list of current holder names in the io.argoproj.workflow.v1alpha1.
  name: holders
  type: array
- description: Semaphore stores the semaphore name.
  name: semaphore
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-holding-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-holding
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-holding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-holding-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.SemaphoreHolding\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.SemaphoreHolding schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"holders\": {\n      \"description\": \"Holders stores the list of current holder names in the io.argoproj.workflow.v1alpha1.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"semaphore\": {\n      \"description\": \"Semaphore stores the semaphore name.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-holding-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.SemaphoreHolding
---
