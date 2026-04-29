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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-inputs-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Inputs\",\n  \"description\": \"Inputs are the mechanism for passing parameters, artifacts, volumes from one template to another\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"artifacts\": {\n      \"description\": \"Artifact are a list of artifacts passed as inputs\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Artifact\"\n      },\n      \"x-kubernetes-patch-merge-key\": \"name\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    },\n    \"parameters\": {\n      \"description\": \"Parameters are a list of parameters passed as inputs MaxItems is an artificial limit to limit CEL validation costs - see note at top\
  \ of file\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Parameter\"\n      },\n      \"x-kubernetes-patch-merge-key\": \"name\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-inputs-schema.json
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
