---
description: Metadata for list responses including pagination tokens.
layout: schema
name: ListMeta
properties_list:
- description: ''
  name: selfLink
  type: string
- description: ''
  name: resourceVersion
  type: string
- description: ''
  name: continue
  type: string
- description: ''
  name: remainingItemCount
  type: integer
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-list-meta-schema.json
slug: openshift-rest-list-meta
source_filename: openshift-rest-list-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListMeta\",\n  \"type\": \"object\",\n  \"description\": \"Metadata for list responses including pagination tokens.\",\n  \"properties\": {\n    \"selfLink\": {\n      \"type\": \"string\"\n    },\n    \"resourceVersion\": {\n      \"type\": \"string\"\n    },\n    \"continue\": {\n      \"type\": \"string\"\n    },\n    \"remainingItemCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-list-meta-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: ListMeta
---
