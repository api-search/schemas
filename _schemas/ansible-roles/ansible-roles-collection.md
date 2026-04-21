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
