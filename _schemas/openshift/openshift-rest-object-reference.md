---
description: A reference to a Kubernetes object.
layout: schema
name: ObjectReference
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-object-reference-schema.json
slug: openshift-rest-object-reference
source_filename: openshift-rest-object-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectReference\",\n  \"type\": \"object\",\n  \"description\": \"A reference to a Kubernetes object.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-object-reference-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: ObjectReference
---
