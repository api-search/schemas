---
description: A paginated list of repositories.
layout: schema
name: RepositoryList
properties_list:
- description: ''
  name: repositories
  type: array
- description: The pagination token for the next page.
  name: next_page
  type: string
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-quay-repository-list-schema.json
slug: red-hat-quay-repository-list
source_filename: red-hat-quay-repository-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RepositoryList\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of repositories.\",\n  \"properties\": {\n    \"repositories\": {\n      \"type\": \"array\"\n    },\n    \"next_page\": {\n      \"type\": \"string\",\n      \"description\": \"The pagination token for the next page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-quay-repository-list-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: RepositoryList
---
