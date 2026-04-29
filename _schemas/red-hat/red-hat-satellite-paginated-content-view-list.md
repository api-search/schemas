---
description: ''
layout: schema
name: PaginatedContentViewList
properties_list:
- description: ''
  name: total
  type: integer
- description: ''
  name: subtotal
  type: integer
- description: ''
  name: page
  type: integer
- description: ''
  name: per_page
  type: integer
- description: ''
  name: results
  type: array
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-satellite-paginated-content-view-list-schema.json
slug: red-hat-satellite-paginated-content-view-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaginatedContentViewList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"subtotal\": {\n      \"type\": \"integer\"\n    },\n    \"page\": {\n      \"type\": \"integer\"\n    },\n    \"per_page\": {\n      \"type\": \"integer\"\n    },\n    \"results\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-satellite-paginated-content-view-list-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: PaginatedContentViewList
---
