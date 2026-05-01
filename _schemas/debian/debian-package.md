---
description: A Debian source package with name, version, and metadata.
layout: schema
name: Debian Source Package
properties_list:
- description: ''
  name: package
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: suites
  type: array
- description: ''
  name: maintainer
  type: string
- description: ''
  name: uploaders
  type: array
- description: ''
  name: section
  type: string
- description: ''
  name: priority
  type: string
- description: ''
  name: homepage
  type: string
- description: ''
  name: vcs_browser
  type: string
- description: ''
  name: vcs_git
  type: string
provider_name: Debian
provider_slug: debian
schema_file: json-schema/debian-package.json
slug: debian-package
source_filename: debian-package.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/debian/json-schema/debian-package.json\",\n  \"title\": \"Debian Source Package\",\n  \"description\": \"A Debian source package with name, version, and metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"package\": {\"type\": \"string\"},\n    \"version\": {\"type\": \"string\"},\n    \"suites\": {\"type\": \"array\", \"items\": {\"type\": \"string\"}},\n    \"maintainer\": {\"type\": \"string\"},\n    \"uploaders\": {\"type\": \"array\", \"items\": {\"type\": \"string\"}},\n    \"section\": {\"type\": \"string\"},\n    \"priority\": {\"type\": \"string\"},\n    \"homepage\": {\"type\": \"string\", \"format\": \"uri\"},\n    \"vcs_browser\": {\"type\": \"string\", \"format\": \"uri\"},\n    \"vcs_git\": {\"type\": \"string\"}\n  },\n  \"required\": [\"package\", \"version\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/debian/refs/heads/main/json-schema/debian-package.json
tags:
- Bug Tracker
- Debian
- Linux
- Open Source
- Operating System
- Package Management
- Source Code
title: Debian Source Package
---
