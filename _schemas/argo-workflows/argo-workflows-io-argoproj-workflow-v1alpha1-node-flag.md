---
description: io.argoproj.workflow.v1alpha1.NodeFlag schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.NodeFlag
properties_list:
- description: Hooked tracks whether or not this node was triggered by hook or onExit
  name: hooked
  type: boolean
- description: Retried tracks whether or not this node was retried by retryStrategy
  name: retried
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-node-flag-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-node-flag
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-node-flag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-node-flag-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.NodeFlag\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.NodeFlag schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hooked\": {\n      \"description\": \"Hooked tracks whether or not this node was triggered by hook or onExit\",\n      \"type\": \"boolean\"\n    },\n    \"retried\": {\n      \"description\": \"Retried tracks whether or not this node was retried by retryStrategy\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-node-flag-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.NodeFlag
---
