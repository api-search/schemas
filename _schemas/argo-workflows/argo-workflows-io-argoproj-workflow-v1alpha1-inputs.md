---
description: Inputs are the mechanism for passing parameters, artifacts, volumes from one template to another
layout: schema
name: io.argoproj.workflow.v1alpha1.Inputs
properties_list:
- description: Artifact are a list of artifacts passed as inputs
  name: artifacts
  type: array
- description: Parameters are a list of parameters passed as inputs MaxItems is an artificial limit to limit CEL validation costs - see note at top of file
  name: parameters
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-inputs-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-inputs
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Inputs
---
