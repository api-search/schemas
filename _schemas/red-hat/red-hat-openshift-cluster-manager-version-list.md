---
description: A paginated list of available OpenShift versions.
layout: schema
name: VersionList
properties_list:
- description: ''
  name: kind
  type: string
- description: ''
  name: page
  type: integer
- description: ''
  name: size
  type: integer
- description: ''
  name: total
  type: integer
- description: ''
  name: items
  type: array
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-openshift-cluster-manager-version-list-schema.json
slug: red-hat-openshift-cluster-manager-version-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VersionList\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of available OpenShift versions.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"page\": {\n      \"type\": \"integer\"\n    },\n    \"size\": {\n      \"type\": \"integer\"\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"items\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-openshift-cluster-manager-version-list-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: VersionList
---
