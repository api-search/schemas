---
description: StopStrategy defines if the CronWorkflow should stop scheduling based on an expression. v3.6 and after
layout: schema
name: io.argoproj.workflow.v1alpha1.StopStrategy
properties_list:
- description: 'v3.6 and after: Expression is an expression that stops scheduling workflows when true. Use the variables `cronworkflow`.`failed` or `cronworkflow`.`succeeded` to access the number of failed or success'
  name: expression
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-stop-strategy-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-stop-strategy
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-stop-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-stop-strategy-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.StopStrategy\",\n  \"description\": \"StopStrategy defines if the CronWorkflow should stop scheduling based on an expression. v3.6 and after\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expression\": {\n      \"description\": \"v3.6 and after: Expression is an expression that stops scheduling workflows when true. Use the variables `cronworkflow`.`failed` or `cronworkflow`.`succeeded` to access the number of failed or successful child workflows.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"expression\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-stop-strategy-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.StopStrategy
---
