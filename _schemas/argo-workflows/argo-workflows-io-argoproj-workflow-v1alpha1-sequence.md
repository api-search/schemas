---
description: Sequence expands a workflow step into numeric range
layout: schema
name: io.argoproj.workflow.v1alpha1.Sequence
properties_list:
- description: 'Count is number of elements in the sequence (default: 0). Not to be used with end'
  name: count
  type: object
- description: 'Number at which to end the sequence (default: 0). Not to be used with Count'
  name: end
  type: object
- description: Format is a printf format string to format the value in the sequence
  name: format
  type: string
- description: 'Number at which to start the sequence (default: 0)'
  name: start
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-sequence-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-sequence
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-sequence-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-sequence-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Sequence\",\n  \"description\": \"Sequence expands a workflow step into numeric range\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"description\": \"Count is number of elements in the sequence (default: 0). Not to be used with end\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.util.intstr.IntOrString\"\n    },\n    \"end\": {\n      \"description\": \"Number at which to end the sequence (default: 0). Not to be used with Count\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.util.intstr.IntOrString\"\n    },\n    \"format\": {\n      \"description\": \"Format is a printf format string to format the value in the sequence\",\n      \"type\"\
  : \"string\"\n    },\n    \"start\": {\n      \"description\": \"Number at which to start the sequence (default: 0)\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.util.intstr.IntOrString\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-sequence-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Sequence
---
