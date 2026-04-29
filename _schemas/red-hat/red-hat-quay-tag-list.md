---
description: A paginated list of image tags.
layout: schema
name: TagList
properties_list:
- description: ''
  name: tags
  type: array
- description: ''
  name: page
  type: integer
- description: ''
  name: has_additional
  type: boolean
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-quay-tag-list-schema.json
slug: red-hat-quay-tag-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagList\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of image tags.\",\n  \"properties\": {\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"page\": {\n      \"type\": \"integer\"\n    },\n    \"has_additional\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-quay-tag-list-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: TagList
---
