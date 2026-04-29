---
description: Column is a custom column that will be exposed in the Workflow List View.
layout: schema
name: io.argoproj.workflow.v1alpha1.Column
properties_list:
- description: The key of the label or annotation, e.g., "workflows.argoproj.io/completed".
  name: key
  type: string
- description: The name of this column, e.g., "Workflow Completed".
  name: name
  type: string
- description: The type of this column, "label" or "annotation".
  name: type
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-column-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-column
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-column-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-column-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Column\",\n  \"description\": \"Column is a custom column that will be exposed in the Workflow List View.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"description\": \"The key of the label or annotation, e.g., \\\"workflows.argoproj.io/completed\\\".\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of this column, e.g., \\\"Workflow Completed\\\".\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of this column, \\\"label\\\" or \\\"annotation\\\".\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\",\n    \"key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-column-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Column
---
