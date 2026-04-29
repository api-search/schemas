---
description: A generic paginated list response.
layout: schema
name: PaginatedList
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: next
  type: string
- description: ''
  name: previous
  type: string
- description: ''
  name: results
  type: array
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-ansible-automation-platform-paginated-list-schema.json
slug: red-hat-ansible-automation-platform-paginated-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaginatedList\",\n  \"type\": \"object\",\n  \"description\": \"A generic paginated list response.\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\"\n    },\n    \"next\": {\n      \"type\": \"string\"\n    },\n    \"previous\": {\n      \"type\": \"string\"\n    },\n    \"results\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-ansible-automation-platform-paginated-list-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: PaginatedList
---
