---
description: Sequence expands a workflow step into numeric range
layout: schema
name: io.argoproj.workflow.v1alpha1.Sequence
properties_list:
- description: 'Count is number of elements in the sequence (default: 0). Not to be used with end'
  name: count
  type: object
- description: 'Number at which to end the sequence (default: 0). Not to be used with Count'
  name: end
  type: object
- description: Format is a printf format string to format the value in the sequence
  name: format
  type: string
- description: 'Number at which to start the sequence (default: 0)'
  name: start
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-sequence-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-sequence
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Sequence
---
