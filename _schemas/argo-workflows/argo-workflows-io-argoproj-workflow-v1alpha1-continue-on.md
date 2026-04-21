---
description: ContinueOn defines if a workflow should continue even if a task or step fails/errors. It can be specified if the workflow should continue when the pod errors, fails or both.
layout: schema
name: io.argoproj.workflow.v1alpha1.ContinueOn
properties_list:
- description: ''
  name: error
  type: boolean
- description: ''
  name: failed
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-continue-on-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-continue-on
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ContinueOn
---
