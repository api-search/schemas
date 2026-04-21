---
description: EventDependencyFilter defines filters and constraints for a io.argoproj.workflow.v1alpha1.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventDependencyFilter
properties_list:
- description: ''
  name: context
  type: object
- description: ''
  name: data
  type: array
- description: 'DataLogicalOperator defines how multiple Data filters (if defined) are evaluated together. Available values: and (&&), or (||) Is optional and if left blank treated as and (&&).'
  name: dataLogicalOperator
  type: string
- description: 'ExprLogicalOperator defines how multiple Exprs filters (if defined) are evaluated together. Available values: and (&&), or (||) Is optional and if left blank treated as and (&&).'
  name: exprLogicalOperator
  type: string
- description: Exprs contains the list of expressions evaluated against the event payload.
  name: exprs
  type: array
- description: Script refers to a Lua script evaluated to determine the validity of an io.argoproj.workflow.v1alpha1.
  name: script
  type: string
- description: ''
  name: time
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-dependency-filter-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-dependency-filter
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventDependencyFilter
---
