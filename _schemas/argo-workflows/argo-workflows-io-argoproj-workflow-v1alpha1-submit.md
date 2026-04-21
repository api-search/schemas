---
description: io.argoproj.workflow.v1alpha1.Submit schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.Submit
properties_list:
- description: Arguments extracted from the event and then set as arguments to the workflow created.
  name: arguments
  type: object
- description: Metadata optional means to customize select fields of the workflow metadata
  name: metadata
  type: object
- description: WorkflowTemplateRef the workflow template to submit
  name: workflowTemplateRef
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-submit-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-submit
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Submit
---
