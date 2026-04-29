---
description: Status is a return value for calls that do not return other objects.
layout: schema
name: Status
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: reason
  type: string
- description: ''
  name: code
  type: integer
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-status-schema.json
slug: openshift-rest-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status\",\n  \"type\": \"object\",\n  \"description\": \"Status is a return value for calls that do not return other objects.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"type\": \"string\"\n    },\n    \"code\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-status-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: Status
---
