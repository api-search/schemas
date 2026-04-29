---
description: Pagination links for navigating result sets.
layout: schema
name: PaginationLinks
properties_list:
- description: URL to the first page.
  name: first
  type: string
- description: URL to the last page.
  name: last
  type: string
- description: URL to the next page.
  name: next
  type: string
- description: URL to the previous page.
  name: previous
  type: string
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-insights-pagination-links-schema.json
slug: red-hat-insights-pagination-links
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaginationLinks\",\n  \"type\": \"object\",\n  \"description\": \"Pagination links for navigating result sets.\",\n  \"properties\": {\n    \"first\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the first page.\"\n    },\n    \"last\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the last page.\"\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the next page.\"\n    },\n    \"previous\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the previous page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-insights-pagination-links-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: PaginationLinks
---
