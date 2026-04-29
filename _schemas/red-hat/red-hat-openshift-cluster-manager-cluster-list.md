---
description: A paginated list of clusters.
layout: schema
name: ClusterList
properties_list:
- description: The resource kind.
  name: kind
  type: string
- description: The current page number.
  name: page
  type: integer
- description: The number of items in this page.
  name: size
  type: integer
- description: The total number of items across all pages.
  name: total
  type: integer
- description: The list of clusters.
  name: items
  type: array
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-openshift-cluster-manager-cluster-list-schema.json
slug: red-hat-openshift-cluster-manager-cluster-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterList\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of clusters.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The resource kind.\"\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"The current page number.\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items in this page.\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of items across all pages.\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The list of clusters.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-openshift-cluster-manager-cluster-list-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: ClusterList
---
