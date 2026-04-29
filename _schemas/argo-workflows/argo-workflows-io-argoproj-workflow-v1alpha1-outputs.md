---
description: Outputs hold parameters, artifacts, and results from a step
layout: schema
name: io.argoproj.workflow.v1alpha1.Outputs
properties_list:
- description: Artifacts holds the list of output artifacts produced by a step
  name: artifacts
  type: array
- description: ExitCode holds the exit code of a script template
  name: exitCode
  type: string
- description: Parameters holds the list of output parameters produced by a step
  name: parameters
  type: array
- description: Result holds the result (stdout) of a script or container template, or the response body of an HTTP template
  name: result
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-outputs-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-outputs
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-outputs-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-outputs-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Outputs\",\n  \"description\": \"Outputs hold parameters, artifacts, and results from a step\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"artifacts\": {\n      \"description\": \"Artifacts holds the list of output artifacts produced by a step\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Artifact\"\n      },\n      \"x-kubernetes-patch-merge-key\": \"name\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    },\n    \"exitCode\": {\n      \"description\": \"ExitCode holds the exit code of a script template\",\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"description\": \"Parameters holds\
  \ the list of output parameters produced by a step\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Parameter\"\n      },\n      \"x-kubernetes-patch-merge-key\": \"name\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    },\n    \"result\": {\n      \"description\": \"Result holds the result (stdout) of a script or container template, or the response body of an HTTP template\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-outputs-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Outputs
---
