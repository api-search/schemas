---
description: Arguments to a template
layout: schema
name: io.argoproj.workflow.v1alpha1.Arguments
properties_list:
- description: Artifacts is the list of artifacts to pass to the template or workflow
  name: artifacts
  type: array
- description: Parameters is the list of parameters to pass to the template or workflow
  name: parameters
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-arguments-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-arguments
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-arguments-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-arguments-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Arguments\",\n  \"description\": \"Arguments to a template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"artifacts\": {\n      \"description\": \"Artifacts is the list of artifacts to pass to the template or workflow\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Artifact\"\n      },\n      \"x-kubernetes-patch-merge-key\": \"name\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    },\n    \"parameters\": {\n      \"description\": \"Parameters is the list of parameters to pass to the template or workflow\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Parameter\"\
  \n      },\n      \"x-kubernetes-patch-merge-key\": \"name\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-arguments-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Arguments
---
