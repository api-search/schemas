---
description: SuspendTemplate is a template subtype to suspend a workflow at a predetermined point in time
layout: schema
name: io.argoproj.workflow.v1alpha1.SuspendTemplate
properties_list:
- description: 'Duration is the seconds to wait before automatically resuming a template. Must be a string. Default unit is seconds. Could also be a Duration, e.g.: "2m", "6h"'
  name: duration
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-suspend-template-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-suspend-template
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.SuspendTemplate
---
