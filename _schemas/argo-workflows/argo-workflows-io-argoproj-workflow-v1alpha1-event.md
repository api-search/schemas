---
description: io.argoproj.workflow.v1alpha1.Event schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.Event
properties_list:
- description: Selector (https://github.com/expr-lang/expr) that we must must match the io.argoproj.workflow.v1alpha1. E.g. `payload.message == "test"`
  name: selector
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-event-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-event
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-event-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Event\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.Event schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"selector\": {\n      \"description\": \"Selector (https://github.com/expr-lang/expr) that we must must match the io.argoproj.workflow.v1alpha1. E.g. `payload.message == \\\"test\\\"`\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"selector\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-event-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Event
---
