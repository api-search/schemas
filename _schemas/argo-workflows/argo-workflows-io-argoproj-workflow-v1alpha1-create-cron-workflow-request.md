---
description: io.argoproj.workflow.v1alpha1.CreateCronWorkflowRequest schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.CreateCronWorkflowRequest
properties_list:
- description: ''
  name: createOptions
  type: object
- description: ''
  name: cronWorkflow
  type: object
- description: ''
  name: namespace
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-create-cron-workflow-request-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-create-cron-workflow-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-create-cron-workflow-request-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.CreateCronWorkflowRequest\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.CreateCronWorkflowRequest schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createOptions\": {\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.CreateOptions\"\n    },\n    \"cronWorkflow\": {\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.CronWorkflow\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-create-cron-workflow-request-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.CreateCronWorkflowRequest
---
