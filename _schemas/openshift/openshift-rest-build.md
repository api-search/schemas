---
description: A Build represents a single execution of a build process that transforms source code into a runnable container image. Builds are created from BuildConfigs or instantiated directly.
layout: schema
name: Build
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-build-schema.json
slug: openshift-rest-build
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Build\",\n  \"type\": \"object\",\n  \"description\": \"A Build represents a single execution of a build process that transforms source code into a runnable container image. Builds are created from BuildConfigs or instantiated directly.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-build-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: Build
---
