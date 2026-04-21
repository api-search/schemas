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
