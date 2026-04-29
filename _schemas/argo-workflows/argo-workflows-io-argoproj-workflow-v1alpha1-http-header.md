---
description: io.argoproj.workflow.v1alpha1.HTTPHeader schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.HTTPHeader
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: value
  type: string
- description: ''
  name: valueFrom
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-http-header-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-http-header
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-http-header-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-http-header-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.HTTPHeader\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.HTTPHeader schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"string\"\n    },\n    \"valueFrom\": {\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.HTTPHeaderSource\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-http-header-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.HTTPHeader
---
