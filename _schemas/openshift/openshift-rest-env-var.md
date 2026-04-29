---
description: An environment variable to set in a container.
layout: schema
name: EnvVar
properties_list:
- description: The environment variable name.
  name: name
  type: string
- description: The environment variable value.
  name: value
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-env-var-schema.json
slug: openshift-rest-env-var
source_filename: openshift-rest-env-var-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvVar\",\n  \"type\": \"object\",\n  \"description\": \"An environment variable to set in a container.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The environment variable name.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The environment variable value.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-env-var-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: EnvVar
---
