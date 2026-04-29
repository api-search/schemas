---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ArgoWorkflowTrigger schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ArgoWorkflowTrigger
properties_list:
- description: ''
  name: args
  type: array
- description: ''
  name: operation
  type: string
- description: ''
  name: parameters
  type: array
- description: ''
  name: source
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-argo-workflow-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-argo-workflow-trigger
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-argo-workflow-trigger-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ArgoWorkflowTrigger\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ArgoWorkflowTrigger schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"args\": {\n      \"type\": \"array\",\n      \"title\": \"Args is the list of arguments to pass to the argo CLI\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"operation\": {\n      \"type\": \"string\",\n      \"title\": \"Operation refers to the type of operation performed on the argo workflow resource.\\nDefault value is Submit.\\n+optional\"\n    },\n    \"parameters\": {\n      \"type\"\
  : \"array\",\n      \"title\": \"Parameters is the list of parameters to pass to resolved Argo Workflow object\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"source\": {\n      \"title\": \"Source of the K8s resource file(s)\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ArtifactLocation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-argo-workflow-trigger-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ArgoWorkflowTrigger
---
