---
description: Schema describing a container image repository in Quay.
layout: schema
name: Quay Repository
properties_list:
- description: Owning user or organization namespace.
  name: namespace
  type: string
- description: Repository name within the namespace.
  name: name
  type: string
- description: Markdown description of the repository.
  name: description
  type: string
- description: ''
  name: visibility
  type: string
- description: ''
  name: is_organization
  type: boolean
- description: ''
  name: is_starred
  type: boolean
- description: ''
  name: kind
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: trust_enabled
  type: boolean
- description: Default tag expiration in seconds.
  name: tag_expiration_s
  type: integer
- description: Unix timestamp of last modification.
  name: last_modified
  type:
  - integer
  - 'null'
provider_name: Quay
provider_slug: quay
schema_file: json-schema/quay-repository-schema.json
slug: quay-repository
source_filename: quay-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/json-schema/quay-repository-schema.json\",\n  \"title\": \"Quay Repository\",\n  \"description\": \"Schema describing a container image repository in Quay.\",\n  \"type\": \"object\",\n  \"required\": [\"namespace\", \"name\"],\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Owning user or organization namespace.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Repository name within the namespace.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Markdown description of the repository.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\"public\", \"private\"]\n    },\n    \"is_organization\": {\n      \"type\": \"boolean\"\n    },\n    \"is_starred\": {\n      \"type\": \"boolean\"\
  \n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"enum\": [\"image\", \"application\"]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"NORMAL\", \"READ_ONLY\", \"MIRROR\"]\n    },\n    \"trust_enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"tag_expiration_s\": {\n      \"type\": \"integer\",\n      \"description\": \"Default tag expiration in seconds.\"\n    },\n    \"last_modified\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Unix timestamp of last modification.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/json-schema/quay-repository-schema.json
tags:
- Container Images
- Containers
- Red Hat
- Registry
- Security Scanning
title: Quay Repository
---
