---
description: EnvFromSource represents the source of a set of ConfigMaps or Secrets
layout: schema
name: io.k8s.api.core.v1.EnvFromSource
properties_list:
- description: The ConfigMap to select from
  name: configMapRef
  type: object
- description: Optional text to prepend to the name of each environment variable. May consist of any printable ASCII characters except '='.
  name: prefix
  type: string
- description: The Secret to select from
  name: secretRef
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-env-from-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-env-from-source
source_filename: argo-workflows-io-k8s-api-core-v1-env-from-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-env-from-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.EnvFromSource\",\n  \"description\": \"EnvFromSource represents the source of a set of ConfigMaps or Secrets\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configMapRef\": {\n      \"description\": \"The ConfigMap to select from\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ConfigMapEnvSource\"\n    },\n    \"prefix\": {\n      \"description\": \"Optional text to prepend to the name of each environment variable. May consist of any printable ASCII characters except '='.\",\n      \"type\": \"string\"\n    },\n    \"secretRef\": {\n      \"description\": \"The Secret to select from\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretEnvSource\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-env-from-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.EnvFromSource
---
