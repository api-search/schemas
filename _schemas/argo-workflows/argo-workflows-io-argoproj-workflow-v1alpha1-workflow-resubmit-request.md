---
description: io.argoproj.workflow.v1alpha1.WorkflowResubmitRequest schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.WorkflowResubmitRequest
properties_list:
- description: ''
  name: memoized
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: parameters
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-resubmit-request-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-resubmit-request
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-resubmit-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-resubmit-request-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.WorkflowResubmitRequest\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.WorkflowResubmitRequest schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"memoized\": {\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-resubmit-request-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.WorkflowResubmitRequest
---
