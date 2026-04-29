---
description: Docker build strategy that uses a Dockerfile to build images.
layout: schema
name: DockerBuildStrategy
properties_list:
- description: Path of the Dockerfile relative to the context directory.
  name: dockerfilePath
  type: string
- description: ''
  name: env
  type: array
- description: If true, Docker build caching is disabled.
  name: noCache
  type: boolean
- description: Forces a pull of the base image before the build.
  name: forcePull
  type: boolean
- description: Specifies build arguments to pass to Docker.
  name: buildArgs
  type: array
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-docker-build-strategy-schema.json
slug: openshift-rest-docker-build-strategy
source_filename: openshift-rest-docker-build-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DockerBuildStrategy\",\n  \"type\": \"object\",\n  \"description\": \"Docker build strategy that uses a Dockerfile to build images.\",\n  \"properties\": {\n    \"dockerfilePath\": {\n      \"type\": \"string\",\n      \"description\": \"Path of the Dockerfile relative to the context directory.\"\n    },\n    \"env\": {\n      \"type\": \"array\"\n    },\n    \"noCache\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, Docker build caching is disabled.\"\n    },\n    \"forcePull\": {\n      \"type\": \"boolean\",\n      \"description\": \"Forces a pull of the base image before the build.\"\n    },\n    \"buildArgs\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies build arguments to pass to Docker.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-docker-build-strategy-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: DockerBuildStrategy
---
