---
description: A paginated list of job templates.
layout: schema
name: PaginatedJobTemplateList
properties_list:
- description: The total number of results.
  name: count
  type: integer
- description: URL to the next page of results.
  name: next
  type: string
- description: URL to the previous page of results.
  name: previous
  type: string
- description: ''
  name: results
  type: array
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-ansible-automation-platform-paginated-job-template-list-schema.json
slug: red-hat-ansible-automation-platform-paginated-job-template-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaginatedJobTemplateList\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of job templates.\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of results.\"\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the next page of results.\"\n    },\n    \"previous\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the previous page of results.\"\n    },\n    \"results\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-ansible-automation-platform-paginated-job-template-list-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: PaginatedJobTemplateList
---
