---
description: io.argoproj.workflow.v1alpha1.WorkflowEventBindingSpec schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.WorkflowEventBindingSpec
properties_list:
- description: Event is the event to bind to
  name: event
  type: object
- description: Submit is the workflow template to submit
  name: submit
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-event-binding-spec-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-event-binding-spec
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-event-binding-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-event-binding-spec-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.WorkflowEventBindingSpec\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.WorkflowEventBindingSpec schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"event\": {\n      \"description\": \"Event is the event to bind to\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Event\"\n    },\n    \"submit\": {\n      \"description\": \"Submit is the workflow template to submit\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Submit\"\n    }\n  },\n  \"required\": [\n    \"event\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-event-binding-spec-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.WorkflowEventBindingSpec
---
