---
description: Contains information to identify an owning object.
layout: schema
name: OwnerReference
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
  name: uid
  type: string
- description: ''
  name: controller
  type: boolean
- description: ''
  name: blockOwnerDeletion
  type: boolean
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-owner-reference-schema.json
slug: openshift-rest-owner-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OwnerReference\",\n  \"type\": \"object\",\n  \"description\": \"Contains information to identify an owning object.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"uid\": {\n      \"type\": \"string\"\n    },\n    \"controller\": {\n      \"type\": \"boolean\"\n    },\n    \"blockOwnerDeletion\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-owner-reference-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: OwnerReference
---
