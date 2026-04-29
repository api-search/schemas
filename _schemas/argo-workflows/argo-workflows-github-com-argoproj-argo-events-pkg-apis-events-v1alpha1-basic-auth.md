---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BasicAuth schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BasicAuth
properties_list:
- description: Password refers to the Kubernetes secret that holds the password required for basic auth.
  name: password
  type: object
- description: Username refers to the Kubernetes secret that holds the username required for basic auth.
  name: username
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-basic-auth-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-basic-auth
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-basic-auth-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-basic-auth-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BasicAuth\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BasicAuth schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"password\": {\n      \"description\": \"Password refers to the Kubernetes secret that holds the password required for basic auth.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"username\": {\n      \"description\": \"Username refers to the Kubernetes secret that holds the username required for basic auth.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-basic-auth-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BasicAuth
---
