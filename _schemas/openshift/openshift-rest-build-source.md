---
description: Specifies the source code location and type for the build input.
layout: schema
name: BuildSource
properties_list:
- description: The type of source input.
  name: type
  type: string
- description: Git source location.
  name: git
  type: object
- description: The Dockerfile content used as build input.
  name: dockerfile
  type: string
- description: The subdirectory within the source repository used as the context for the build.
  name: contextDir
  type: string
- description: Secret holding credentials for accessing the source repository.
  name: sourceSecret
  type: object
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-build-source-schema.json
slug: openshift-rest-build-source
source_filename: openshift-rest-build-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BuildSource\",\n  \"type\": \"object\",\n  \"description\": \"Specifies the source code location and type for the build input.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of source input.\"\n    },\n    \"git\": {\n      \"type\": \"object\",\n      \"description\": \"Git source location.\"\n    },\n    \"dockerfile\": {\n      \"type\": \"string\",\n      \"description\": \"The Dockerfile content used as build input.\"\n    },\n    \"contextDir\": {\n      \"type\": \"string\",\n      \"description\": \"The subdirectory within the source repository used as the context for the build.\"\n    },\n    \"sourceSecret\": {\n      \"type\": \"object\",\n      \"description\": \"Secret holding credentials for accessing the source repository.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-build-source-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: BuildSource
---
