---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSAuth schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSAuth
properties_list:
- description: ''
  name: basic
  type: object
- description: ''
  name: credential
  type: object
- description: ''
  name: nkey
  type: object
- description: ''
  name: token
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-auth-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-auth
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-auth-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-auth-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSAuth\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSAuth schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"basic\": {\n      \"title\": \"Baisc auth with username and password\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BasicAuth\"\n    },\n    \"credential\": {\n      \"title\": \"credential used to connect\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"nkey\": {\n      \"title\": \"NKey used to connect\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\
  \n    },\n    \"token\": {\n      \"title\": \"Token used to connect\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-auth-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSAuth
---
