---
description: Schema describing a tag pointing at a manifest in a Quay repository.
layout: schema
name: Quay Tag
properties_list:
- description: Tag name (e.g. latest, v1.0.0).
  name: name
  type: string
- description: Digest of the manifest the tag points at (sha256:...).
  name: manifest_digest
  type: string
- description: ''
  name: is_manifest_list
  type: boolean
- description: ''
  name: size
  type:
  - integer
  - 'null'
- description: ''
  name: last_modified
  type: string
- description: ''
  name: start_ts
  type: integer
- description: ''
  name: end_ts
  type:
  - integer
  - 'null'
- description: ''
  name: expiration
  type:
  - string
  - 'null'
- description: ''
  name: reversion
  type: boolean
provider_name: Quay
provider_slug: quay
schema_file: json-schema/quay-tag-schema.json
slug: quay-tag
source_filename: quay-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/json-schema/quay-tag-schema.json\",\n  \"title\": \"Quay Tag\",\n  \"description\": \"Schema describing a tag pointing at a manifest in a Quay repository.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"manifest_digest\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Tag name (e.g. latest, v1.0.0).\"\n    },\n    \"manifest_digest\": {\n      \"type\": \"string\",\n      \"description\": \"Digest of the manifest the tag points at (sha256:...).\"\n    },\n    \"is_manifest_list\": {\n      \"type\": \"boolean\"\n    },\n    \"size\": {\n      \"type\": [\"integer\", \"null\"]\n    },\n    \"last_modified\": {\n      \"type\": \"string\"\n    },\n    \"start_ts\": {\n      \"type\": \"integer\"\n    },\n    \"end_ts\": {\n      \"type\": [\"integer\", \"null\"]\n    },\n\
  \    \"expiration\": {\n      \"type\": [\"string\", \"null\"]\n    },\n    \"reversion\": {\n      \"type\": \"boolean\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/json-schema/quay-tag-schema.json
tags:
- Container Images
- Containers
- Red Hat
- Registry
- Security Scanning
title: Quay Tag
---
