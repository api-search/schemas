---
description: OAuth2EndpointParam is an optional field that should be sent in the OAuth request.
layout: schema
name: io.argoproj.workflow.v1alpha1.OAuth2EndpointParam
properties_list:
- description: Name is the header name
  name: key
  type: string
- description: Value is the literal value to use for the header
  name: value
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-o-auth2-endpoint-param-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-o-auth2-endpoint-param
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-o-auth2-endpoint-param-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-o-auth2-endpoint-param-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.OAuth2EndpointParam\",\n  \"description\": \"OAuth2EndpointParam is an optional field that should be sent in the OAuth request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"description\": \"Name is the header name\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Value is the literal value to use for the header\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-o-auth2-endpoint-param-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.OAuth2EndpointParam
---
