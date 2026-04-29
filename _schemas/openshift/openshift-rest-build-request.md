---
description: A request to instantiate a new build from a BuildConfig.
layout: schema
name: BuildRequest
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
- description: ''
  name: triggeredBy
  type: array
- description: ''
  name: env
  type: array
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-build-request-schema.json
slug: openshift-rest-build-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BuildRequest\",\n  \"type\": \"object\",\n  \"description\": \"A request to instantiate a new build from a BuildConfig.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"triggeredBy\": {\n      \"type\": \"array\"\n    },\n    \"env\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-build-request-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: BuildRequest
---
