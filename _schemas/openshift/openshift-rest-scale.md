---
description: Represents a scaling request for a resource.
layout: schema
name: Scale
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
- description: ''
  name: spec
  type: object
- description: ''
  name: status
  type: object
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-scale-schema.json
slug: openshift-rest-scale
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Scale\",\n  \"type\": \"object\",\n  \"description\": \"Represents a scaling request for a resource.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"spec\": {\n      \"type\": \"object\"\n    },\n    \"status\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-scale-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: Scale
---
