---
description: A BuildConfig defines the build strategy and source used to produce new container images. Builds can be triggered automatically by webhooks, image changes, or configuration changes.
layout: schema
name: BuildConfig
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-build-config-schema.json
slug: openshift-rest-build-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BuildConfig\",\n  \"type\": \"object\",\n  \"description\": \"A BuildConfig defines the build strategy and source used to produce new container images. Builds can be triggered automatically by webhooks, image changes, or configuration changes.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-build-config-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: BuildConfig
---
