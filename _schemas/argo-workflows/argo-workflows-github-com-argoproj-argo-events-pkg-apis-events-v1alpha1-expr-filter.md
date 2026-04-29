---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ExprFilter schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ExprFilter
properties_list:
- description: Expr refers to the expression that determines the outcome of the filter.
  name: expr
  type: string
- description: Fields refers to set of keys that refer to the paths within event payload.
  name: fields
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-expr-filter-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-expr-filter
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-expr-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-expr-filter-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ExprFilter\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ExprFilter schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expr\": {\n      \"description\": \"Expr refers to the expression that determines the outcome of the filter.\",\n      \"type\": \"string\"\n    },\n    \"fields\": {\n      \"description\": \"Fields refers to set of keys that refer to the paths within event payload.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PayloadField\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-expr-filter-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ExprFilter
---
