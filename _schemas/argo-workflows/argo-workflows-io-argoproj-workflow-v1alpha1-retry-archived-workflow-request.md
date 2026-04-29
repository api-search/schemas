---
description: io.argoproj.workflow.v1alpha1.RetryArchivedWorkflowRequest schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.RetryArchivedWorkflowRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: nodeFieldSelector
  type: string
- description: ''
  name: parameters
  type: array
- description: ''
  name: restartSuccessful
  type: boolean
- description: ''
  name: uid
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-retry-archived-workflow-request-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-retry-archived-workflow-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-retry-archived-workflow-request-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.RetryArchivedWorkflowRequest\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.RetryArchivedWorkflowRequest schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"nodeFieldSelector\": {\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"restartSuccessful\": {\n      \"type\": \"boolean\"\n    },\n    \"uid\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-retry-archived-workflow-request-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.RetryArchivedWorkflowRequest
---
