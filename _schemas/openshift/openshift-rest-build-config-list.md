---
description: A list of BuildConfig objects.
layout: schema
name: BuildConfigList
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
- description: ''
  name: items
  type: array
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-build-config-list-schema.json
slug: openshift-rest-build-config-list
source_filename: openshift-rest-build-config-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BuildConfigList\",\n  \"type\": \"object\",\n  \"description\": \"A list of BuildConfig objects.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"items\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-build-config-list-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: BuildConfigList
---
