---
description: A container image repository in the Quay registry.
layout: schema
name: Repository
properties_list:
- description: The namespace the repository belongs to.
  name: namespace
  type: string
- description: The name of the repository.
  name: name
  type: string
- description: A description of the repository.
  name: description
  type: string
- description: Whether the repository is publicly accessible.
  name: is_public
  type: boolean
- description: The type of repository.
  name: kind
  type: string
- description: The number of tags in the repository.
  name: tag_count
  type: integer
- description: The status token for repository notifications.
  name: status_token
  type: string
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-quay-repository-schema.json
slug: red-hat-quay-repository
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Repository\",\n  \"type\": \"object\",\n  \"description\": \"A container image repository in the Quay registry.\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace the repository belongs to.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the repository.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the repository.\"\n    },\n    \"is_public\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository is publicly accessible.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The type of repository.\"\n    },\n    \"tag_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of tags in the repository.\"\n    },\n    \"status_token\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The status token for repository notifications.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-quay-repository-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Repository
---
