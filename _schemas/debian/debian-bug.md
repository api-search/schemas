---
description: A bug record from the Debian Bug Tracking System (BTS).
layout: schema
name: Debian Bug Report
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: package
  type: string
- description: ''
  name: subject
  type: string
- description: ''
  name: submitter
  type: string
- description: ''
  name: severity
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: tags
  type: array
- description: ''
  name: date
  type: string
- description: ''
  name: last_modified
  type: string
- description: ''
  name: done
  type: string
- description: ''
  name: owner
  type: string
provider_name: Debian
provider_slug: debian
schema_file: json-schema/debian-bug.json
slug: debian-bug
source_filename: debian-bug.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/debian/json-schema/debian-bug.json\",\n  \"title\": \"Debian Bug Report\",\n  \"description\": \"A bug record from the Debian Bug Tracking System (BTS).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\"type\": \"integer\"},\n    \"package\": {\"type\": \"string\"},\n    \"subject\": {\"type\": \"string\"},\n    \"submitter\": {\"type\": \"string\"},\n    \"severity\": {\"type\": \"string\", \"enum\": [\"critical\", \"grave\", \"serious\", \"important\", \"normal\", \"minor\", \"wishlist\"]},\n    \"status\": {\"type\": \"string\"},\n    \"tags\": {\"type\": \"array\", \"items\": {\"type\": \"string\"}},\n    \"date\": {\"type\": \"string\", \"format\": \"date-time\"},\n    \"last_modified\": {\"type\": \"string\", \"format\": \"date-time\"},\n    \"done\": {\"type\": \"string\"},\n    \"owner\": {\"type\": \"string\"}\n  },\n  \"required\": [\"\
  id\", \"package\", \"subject\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/debian/refs/heads/main/json-schema/debian-bug.json
tags:
- Bug Tracker
- Debian
- Linux
- Open Source
- Operating System
- Package Management
- Source Code
title: Debian Bug Report
---
