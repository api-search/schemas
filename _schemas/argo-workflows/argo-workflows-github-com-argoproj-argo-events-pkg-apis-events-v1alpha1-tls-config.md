---
description: TLSConfig refers to TLS configuration for a client.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig
properties_list:
- description: ''
  name: caCertSecret
  type: object
- description: ''
  name: clientCertSecret
  type: object
- description: ''
  name: clientKeySecret
  type: object
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: insecureSkipVerify
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-tls-config-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-tls-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-tls-config-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\",\n  \"description\": \"TLSConfig refers to TLS configuration for a client.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"caCertSecret\": {\n      \"title\": \"CACertSecret refers to the secret that contains the CA cert\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"clientCertSecret\": {\n      \"title\": \"ClientCertSecret refers to the secret that contains the client cert\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"clientKeySecret\": {\n      \"title\": \"ClientKeySecret refers to the secret that contains the client key\",\n\
  \      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"title\": \"Enabled indicates if TLS is enabled. Added for compatibility proposes for Brokers that needs TLS without key authentication\\n+optional\"\n    },\n    \"insecureSkipVerify\": {\n      \"type\": \"boolean\",\n      \"title\": \"If true, skips creation of TLSConfig with certs and creates an empty TLSConfig. (Defaults to false)\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-tls-config-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig
---
