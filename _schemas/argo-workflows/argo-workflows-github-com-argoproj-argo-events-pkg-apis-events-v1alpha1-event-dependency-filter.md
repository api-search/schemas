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
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-dependency-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-dependency-filter-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventDependencyFilter\",\n  \"description\": \"EventDependencyFilter defines filters and constraints for a io.argoproj.workflow.v1alpha1.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"context\": {\n      \"title\": \"Context filter constraints\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventContext\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"title\": \"Data filter constraints with escalation\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.DataFilter\"\n      }\n    },\n    \"dataLogicalOperator\"\
  : {\n      \"description\": \"DataLogicalOperator defines how multiple Data filters (if defined) are evaluated together.\\nAvailable values: and (&&), or (||)\\nIs optional and if left blank treated as and (&&).\",\n      \"type\": \"string\"\n    },\n    \"exprLogicalOperator\": {\n      \"description\": \"ExprLogicalOperator defines how multiple Exprs filters (if defined) are evaluated together.\\nAvailable values: and (&&), or (||)\\nIs optional and if left blank treated as and (&&).\",\n      \"type\": \"string\"\n    },\n    \"exprs\": {\n      \"description\": \"Exprs contains the list of expressions evaluated against the event payload.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ExprFilter\"\n      }\n    },\n    \"script\": {\n      \"description\": \"Script refers to a Lua script evaluated to determine the validity of an io.argoproj.workflow.v1alpha1.\",\n      \"type\": \"string\"\
  \n    },\n    \"time\": {\n      \"title\": \"Time filter on the event with escalation\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TimeFilter\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-dependency-filter-schema.json
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
