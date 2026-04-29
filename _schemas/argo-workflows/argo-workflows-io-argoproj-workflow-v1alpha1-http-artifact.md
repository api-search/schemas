---
description: HTTPArtifact allows a file served on HTTP to be placed as an input artifact in a container
layout: schema
name: io.argoproj.workflow.v1alpha1.HTTPArtifact
properties_list:
- description: Auth contains information for client authentication
  name: auth
  type: object
- description: Headers are an optional list of headers to send with HTTP requests for artifacts
  name: headers
  type: array
- description: URL of the artifact
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-http-artifact-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-http-artifact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-http-artifact-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.HTTPArtifact\",\n  \"description\": \"HTTPArtifact allows a file served on HTTP to be placed as an input artifact in a container\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"auth\": {\n      \"description\": \"Auth contains information for client authentication\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.HTTPAuth\"\n    },\n    \"headers\": {\n      \"description\": \"Headers are an optional list of headers to send with HTTP requests for artifacts\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Header\"\n      }\n    },\n    \"url\": {\n      \"description\": \"URL of the artifact\",\n\
  \      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-http-artifact-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.HTTPArtifact
---
