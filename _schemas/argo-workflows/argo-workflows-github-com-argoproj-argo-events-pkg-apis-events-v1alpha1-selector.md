---
description: Selector represents conditional operation to select K8s objects.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Selector
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: operation
  type: string
- description: ''
  name: value
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-selector-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-selector
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-selector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-selector-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Selector\",\n  \"description\": \"Selector represents conditional operation to select K8s objects.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"title\": \"Key name\"\n    },\n    \"operation\": {\n      \"type\": \"string\",\n      \"title\": \"Supported operations like ==, != etc.\\nDefaults to ==.\\nRefer https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/#label-selectors for more io.argoproj.workflow.v1alpha1.\\n+optional\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"title\": \"Value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-selector-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Selector
---
