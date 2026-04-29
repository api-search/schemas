---
description: Status of the BuildConfig.
layout: schema
name: BuildConfigStatus
properties_list:
- description: The version of the last build created from this config.
  name: lastVersion
  type: integer
- description: ''
  name: imageChangeTriggers
  type: array
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-build-config-status-schema.json
slug: openshift-rest-build-config-status
source_filename: openshift-rest-build-config-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BuildConfigStatus\",\n  \"type\": \"object\",\n  \"description\": \"Status of the BuildConfig.\",\n  \"properties\": {\n    \"lastVersion\": {\n      \"type\": \"integer\",\n      \"description\": \"The version of the last build created from this config.\"\n    },\n    \"imageChangeTriggers\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-build-config-status-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: BuildConfigStatus
---
