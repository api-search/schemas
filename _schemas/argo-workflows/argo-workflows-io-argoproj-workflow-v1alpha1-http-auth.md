---
description: io.argoproj.workflow.v1alpha1.HTTPAuth schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.HTTPAuth
properties_list:
- description: ''
  name: basicAuth
  type: object
- description: ''
  name: clientCert
  type: object
- description: ''
  name: oauth2
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-http-auth-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-http-auth
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-http-auth-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.HTTPAuth\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.HTTPAuth schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"basicAuth\": {\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.BasicAuth\"\n    },\n    \"clientCert\": {\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ClientCertAuth\"\n    },\n    \"oauth2\": {\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.OAuth2Auth\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-http-auth-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.HTTPAuth
---
