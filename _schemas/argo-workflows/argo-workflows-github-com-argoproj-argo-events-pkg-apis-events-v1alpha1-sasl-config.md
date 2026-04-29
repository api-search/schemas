---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SASLConfig schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SASLConfig
properties_list:
- description: ''
  name: mechanism
  type: string
- description: ''
  name: passwordSecret
  type: object
- description: ''
  name: userSecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sasl-config-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sasl-config
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sasl-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sasl-config-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SASLConfig\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SASLConfig schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mechanism\": {\n      \"type\": \"string\",\n      \"title\": \"SASLMechanism is the name of the enabled SASL mechanism.\\nPossible values: OAUTHBEARER, PLAIN (defaults to PLAIN).\\n+optional\"\n    },\n    \"passwordSecret\": {\n      \"title\": \"Password for SASL/PLAIN authentication\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"userSecret\": {\n      \"title\": \"User is the authentication identity (authcid)\
  \ to present for\\nSASL/PLAIN or SASL/SCRAM authentication\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sasl-config-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SASLConfig
---
