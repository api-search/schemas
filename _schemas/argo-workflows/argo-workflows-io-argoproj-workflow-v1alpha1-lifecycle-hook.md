---
description: io.argoproj.workflow.v1alpha1.LifecycleHook schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.LifecycleHook
properties_list:
- description: Arguments hold arguments to the template
  name: arguments
  type: object
- description: Expression is a condition expression for when a node will be retried. If it evaluates to false, the node will not be retried and the retry strategy will be ignored
  name: expression
  type: string
- description: Template is the name of the template to execute by the hook
  name: template
  type: string
- description: TemplateRef is the reference to the template resource to execute by the hook
  name: templateRef
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-lifecycle-hook-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-lifecycle-hook
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.LifecycleHook
---
