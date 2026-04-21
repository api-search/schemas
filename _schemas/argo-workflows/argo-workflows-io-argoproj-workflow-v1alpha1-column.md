---
description: Column is a custom column that will be exposed in the Workflow List View.
layout: schema
name: io.argoproj.workflow.v1alpha1.Column
properties_list:
- description: The key of the label or annotation, e.g., "workflows.argoproj.io/completed".
  name: key
  type: string
- description: The name of this column, e.g., "Workflow Completed".
  name: name
  type: string
- description: The type of this column, "label" or "annotation".
  name: type
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-column-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-column
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Column
---
