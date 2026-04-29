---
description: Custom build strategy that uses a custom builder image to execute an arbitrary build process.
layout: schema
name: CustomBuildStrategy
properties_list:
- description: ''
  name: env
  type: array
- description: If true, the Docker socket is exposed inside the build container.
  name: exposeDockerSocket
  type: boolean
- description: Forces a pull of the custom builder image before the build.
  name: forcePull
  type: boolean
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-custom-build-strategy-schema.json
slug: openshift-rest-custom-build-strategy
source_filename: openshift-rest-custom-build-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CustomBuildStrategy\",\n  \"type\": \"object\",\n  \"description\": \"Custom build strategy that uses a custom builder image to execute an arbitrary build process.\",\n  \"properties\": {\n    \"env\": {\n      \"type\": \"array\"\n    },\n    \"exposeDockerSocket\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the Docker socket is exposed inside the build container.\"\n    },\n    \"forcePull\": {\n      \"type\": \"boolean\",\n      \"description\": \"Forces a pull of the custom builder image before the build.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-custom-build-strategy-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: CustomBuildStrategy
---
