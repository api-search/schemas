---
description: A paginated list of projects.
layout: schema
name: PaginatedProjectList
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
schema_file: json-schema/red-hat-ansible-automation-platform-paginated-project-list-schema.json
slug: red-hat-ansible-automation-platform-paginated-project-list
source_filename: red-hat-ansible-automation-platform-paginated-project-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaginatedProjectList\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of projects.\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\"\n    },\n    \"next\": {\n      \"type\": \"string\"\n    },\n    \"previous\": {\n      \"type\": \"string\"\n    },\n    \"results\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-ansible-automation-platform-paginated-project-list-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: PaginatedProjectList
---
