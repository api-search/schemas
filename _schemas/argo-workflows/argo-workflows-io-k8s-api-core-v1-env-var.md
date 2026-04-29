---
description: EnvVar represents an environment variable present in a Container.
layout: schema
name: io.k8s.api.core.v1.EnvVar
properties_list:
- description: Name of the environment variable. May consist of any printable ASCII characters except '='.
  name: name
  type: string
- description: 'Variable references $(VAR_NAME) are expanded using the previously defined environment variables in the container and any service environment variables. If a variable cannot be resolved, the reference '
  name: value
  type: string
- description: Source for the environment variable's value. Cannot be used if value is not empty.
  name: valueFrom
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-env-var-schema.json
slug: argo-workflows-io-k8s-api-core-v1-env-var
source_filename: argo-workflows-io-k8s-api-core-v1-env-var-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-env-var-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.EnvVar\",\n  \"description\": \"EnvVar represents an environment variable present in a Container.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Name of the environment variable. May consist of any printable ASCII characters except '='.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Variable references $(VAR_NAME) are expanded using the previously defined environment variables in the container and any service environment variables. If a variable cannot be resolved, the reference in the input string will be unchanged. Double $$ are reduced to a single $, which allows for escaping the $(VAR_NAME) syntax: i.e. \\\"$$(VAR_NAME)\\\" will\
  \ produce the string literal \\\"$(VAR_NAME)\\\". Escaped references will never be expanded, regardless of whether the variable exists or not. Defaults to \\\"\\\".\",\n      \"type\": \"string\"\n    },\n    \"valueFrom\": {\n      \"description\": \"Source for the environment variable's value. Cannot be used if value is not empty.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.EnvVarSource\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-env-var-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.EnvVar
---
