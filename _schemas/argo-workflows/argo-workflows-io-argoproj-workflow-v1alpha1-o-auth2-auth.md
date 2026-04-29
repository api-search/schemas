---
description: OAuth2Auth holds all information for client authentication via OAuth2 tokens
layout: schema
name: io.argoproj.workflow.v1alpha1.OAuth2Auth
properties_list:
- description: ''
  name: clientIDSecret
  type: object
- description: ''
  name: clientSecretSecret
  type: object
- description: ''
  name: endpointParams
  type: array
- description: ''
  name: scopes
  type: array
- description: ''
  name: tokenURLSecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-o-auth2-auth-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-o-auth2-auth
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-o-auth2-auth-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-o-auth2-auth-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.OAuth2Auth\",\n  \"description\": \"OAuth2Auth holds all information for client authentication via OAuth2 tokens\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientIDSecret\": {\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"clientSecretSecret\": {\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"endpointParams\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.OAuth2EndpointParam\"\n      }\n    },\n    \"scopes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tokenURLSecret\"\
  : {\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-o-auth2-auth-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.OAuth2Auth
---
