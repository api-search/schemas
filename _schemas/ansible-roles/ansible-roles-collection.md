---
description: An Ansible collection — a distributable package containing roles, modules, plugins, and documentation.
layout: schema
name: Collection
properties_list:
- description: The Galaxy namespace for this collection.
  name: namespace
  type: string
- description: The collection name.
  name: name
  type: string
- description: The current latest version of the collection.
  name: version
  type: string
- description: Short description of what the collection provides.
  name: description
  type: string
- description: Total download count for this collection.
  name: download_count
  type: integer
- description: Whether this collection is Red Hat certified.
  name: certified
  type: boolean
- description: List of SPDX license identifiers.
  name: license
  type: array
- description: Tags categorizing the collection content.
  name: tags
  type: array
- description: Minimum Ansible version required.
  name: requires_ansible
  type: string
- description: Source code repository URL.
  name: repository
  type: string
- description: Link to collection documentation.
  name: documentation
  type: string
- description: When this collection was first published.
  name: created_at
  type: string
- description: When this collection was last updated.
  name: updated_at
  type: string
provider_name: Ansible Roles
provider_slug: ansible-roles
schema_file: json-schema/ansible-roles-collection-schema.json
slug: ansible-roles-collection
source_filename: ansible-roles-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ansible-roles/refs/heads/main/json-schema/ansible-roles-collection-schema.json\",\n  \"title\": \"Collection\",\n  \"description\": \"An Ansible collection — a distributable package containing roles, modules, plugins, and documentation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\"type\": \"string\", \"description\": \"The Galaxy namespace for this collection.\", \"example\": \"community\"},\n    \"name\": {\"type\": \"string\", \"description\": \"The collection name.\", \"example\": \"general\"},\n    \"version\": {\"type\": \"string\", \"description\": \"The current latest version of the collection.\", \"example\": \"8.6.0\"},\n    \"description\": {\"type\": \"string\", \"description\": \"Short description of what the collection provides.\", \"example\": \"A collection of general-purpose Ansible modules and roles.\"\
  },\n    \"download_count\": {\"type\": \"integer\", \"description\": \"Total download count for this collection.\", \"example\": 5000000},\n    \"certified\": {\"type\": \"boolean\", \"description\": \"Whether this collection is Red Hat certified.\", \"example\": false},\n    \"license\": {\"type\": \"array\", \"items\": {\"type\": \"string\"}, \"description\": \"List of SPDX license identifiers.\", \"example\": [\"GPL-3.0-or-later\"]},\n    \"tags\": {\"type\": \"array\", \"items\": {\"type\": \"string\"}, \"description\": \"Tags categorizing the collection content.\", \"example\": [\"networking\", \"cloud\", \"linux\"]},\n    \"requires_ansible\": {\"type\": \"string\", \"description\": \"Minimum Ansible version required.\", \"example\": \">=2.14.0\"},\n    \"repository\": {\"type\": \"string\", \"format\": \"uri\", \"description\": \"Source code repository URL.\", \"example\": \"https://github.com/ansible-collections/community.general\"},\n    \"documentation\": {\"type\": \"string\"\
  , \"format\": \"uri\", \"description\": \"Link to collection documentation.\", \"example\": \"https://docs.ansible.com/ansible/latest/collections/community/general/\"},\n    \"created_at\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"When this collection was first published.\", \"example\": \"2020-01-01T00:00:00Z\"},\n    \"updated_at\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"When this collection was last updated.\", \"example\": \"2026-04-01T00:00:00Z\"}\n  },\n  \"required\": [\"namespace\", \"name\", \"version\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ansible-roles/refs/heads/main/json-schema/ansible-roles-collection-schema.json
tags:
- Ansible
- Automation
- Collections
- Configuration Management
- DevOps
- Infrastructure As Code
- Roles
title: Collection
---
