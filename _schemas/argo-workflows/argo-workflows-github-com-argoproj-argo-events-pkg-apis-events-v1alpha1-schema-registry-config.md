---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SchemaRegistryConfig schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SchemaRegistryConfig
properties_list:
- description: ''
  name: auth
  type: object
- description: ''
  name: schemaId
  type: integer
- description: Schema Registry URL.
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-schema-registry-config-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-schema-registry-config
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-schema-registry-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-schema-registry-config-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SchemaRegistryConfig\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SchemaRegistryConfig schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"auth\": {\n      \"title\": \"SchemaRegistry - basic authentication\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BasicAuth\"\n    },\n    \"schemaId\": {\n      \"type\": \"integer\",\n      \"title\": \"Schema ID\\n+optional\"\n    },\n    \"url\": {\n      \"description\": \"Schema Registry URL.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-schema-registry-config-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SchemaRegistryConfig
---
