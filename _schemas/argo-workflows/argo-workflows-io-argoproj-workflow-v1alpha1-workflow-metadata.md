---
description: io.argoproj.workflow.v1alpha1.WorkflowMetadata schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.WorkflowMetadata
properties_list:
- description: ''
  name: annotations
  type: object
- description: ''
  name: labels
  type: object
- description: ''
  name: labelsFrom
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-metadata-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-metadata
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-metadata-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.WorkflowMetadata\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.WorkflowMetadata schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"annotations\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"labelsFrom\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.LabelValueFrom\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-metadata-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.WorkflowMetadata
---
