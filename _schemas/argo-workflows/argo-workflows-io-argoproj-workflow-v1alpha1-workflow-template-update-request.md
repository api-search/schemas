---
description: io.argoproj.workflow.v1alpha1.WorkflowTemplateUpdateRequest schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.WorkflowTemplateUpdateRequest
properties_list:
- description: 'DEPRECATED: This field is ignored.'
  name: name
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: template
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-template-update-request-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-workflow-template-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-template-update-request-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.WorkflowTemplateUpdateRequest\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.WorkflowTemplateUpdateRequest schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"DEPRECATED: This field is ignored.\",\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"template\": {\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.WorkflowTemplate\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-workflow-template-update-request-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.WorkflowTemplateUpdateRequest
---
