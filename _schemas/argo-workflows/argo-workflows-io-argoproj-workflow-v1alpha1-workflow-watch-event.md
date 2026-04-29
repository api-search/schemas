---
description: io.argoproj.workflow.v1alpha1.WorkflowWatchEvent schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.WorkflowWatchEvent
properties_list:
- description: ''
  name: object
  type: object
- description: ''
  name: type
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-watch-event-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-watch-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-watch-event-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.WorkflowWatchEvent\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.WorkflowWatchEvent schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"title\": \"the workflow\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Workflow\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"title\": \"the type of change\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-watch-event-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.WorkflowWatchEvent
---
