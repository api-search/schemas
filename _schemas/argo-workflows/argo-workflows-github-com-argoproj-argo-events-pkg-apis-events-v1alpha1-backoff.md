---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Backoff schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Backoff
properties_list:
- description: ''
  name: duration
  type: object
- description: ''
  name: factor
  type: object
- description: ''
  name: jitter
  type: object
- description: ''
  name: steps
  type: integer
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-backoff-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-backoff
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-backoff-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-backoff-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Backoff\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Backoff schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"duration\": {\n      \"title\": \"The initial duration in nanoseconds or strings like \\\"1s\\\", \\\"3m\\\"\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Int64OrString\"\n    },\n    \"factor\": {\n      \"title\": \"Duration is multiplied by factor each iteration\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Amount\"\n    },\n    \"jitter\"\
  : {\n      \"title\": \"The amount of jitter applied each iteration\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Amount\"\n    },\n    \"steps\": {\n      \"type\": \"integer\",\n      \"title\": \"Exit with error after this many steps\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-backoff-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Backoff
---
