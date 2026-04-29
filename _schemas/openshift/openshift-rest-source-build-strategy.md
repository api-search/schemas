---
description: Source-to-Image (S2I) build strategy that combines application source with a builder image to produce a runnable image.
layout: schema
name: SourceBuildStrategy
properties_list:
- description: ''
  name: env
  type: array
- description: URL of S2I scripts to use instead of the ones in the builder image.
  name: scripts
  type: string
- description: Attempt to perform an incremental build reusing artifacts from a prior build.
  name: incremental
  type: boolean
- description: Overrides the default pull behavior and forces a pull of the builder image before the build.
  name: forcePull
  type: boolean
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-source-build-strategy-schema.json
slug: openshift-rest-source-build-strategy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SourceBuildStrategy\",\n  \"type\": \"object\",\n  \"description\": \"Source-to-Image (S2I) build strategy that combines application source with a builder image to produce a runnable image.\",\n  \"properties\": {\n    \"env\": {\n      \"type\": \"array\"\n    },\n    \"scripts\": {\n      \"type\": \"string\",\n      \"description\": \"URL of S2I scripts to use instead of the ones in the builder image.\"\n    },\n    \"incremental\": {\n      \"type\": \"boolean\",\n      \"description\": \"Attempt to perform an incremental build reusing artifacts from a prior build.\"\n    },\n    \"forcePull\": {\n      \"type\": \"boolean\",\n      \"description\": \"Overrides the default pull behavior and forces a pull of the builder image before the build.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-source-build-strategy-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: SourceBuildStrategy
---
