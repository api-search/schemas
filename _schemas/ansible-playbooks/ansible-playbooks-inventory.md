---
description: An Ansible inventory containing groups and hosts targeted by playbook execution.
layout: schema
name: Inventory
properties_list:
- description: Unique identifier for the inventory.
  name: id
  type: integer
- description: Human-readable name for the inventory.
  name: name
  type: string
- description: Description of the inventory and its purpose.
  name: description
  type: string
- description: ID of the organization that owns this inventory.
  name: organization
  type: integer
- description: Inventory kind — empty for standard, smart, or constructed.
  name: kind
  type: string
- description: Filter expression for smart inventories.
  name: host_filter
  type: string
- description: Inventory-level variables as a JSON or YAML string.
  name: variables
  type: string
- description: Total number of hosts in this inventory.
  name: total_hosts
  type: integer
- description: Number of hosts with active failures.
  name: hosts_with_active_failures
  type: integer
- description: Total number of groups in this inventory.
  name: total_groups
  type: integer
- description: Whether this inventory has external inventory sources.
  name: has_inventory_sources
  type: boolean
- description: Timestamp when the inventory was created.
  name: created
  type: string
- description: Timestamp when the inventory was last modified.
  name: modified
  type: string
provider_name: Ansible Playbooks
provider_slug: ansible-playbooks
schema_file: json-schema/ansible-playbooks-inventory-schema.json
slug: ansible-playbooks-inventory
source_filename: ansible-playbooks-inventory-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/json-schema/ansible-playbooks-inventory-schema.json\",\n  \"title\": \"Inventory\",\n  \"description\": \"An Ansible inventory containing groups and hosts targeted by playbook execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\"type\": \"integer\", \"description\": \"Unique identifier for the inventory.\", \"example\": 42},\n    \"name\": {\"type\": \"string\", \"description\": \"Human-readable name for the inventory.\", \"example\": \"Production Web Servers\"},\n    \"description\": {\"type\": \"string\", \"description\": \"Description of the inventory and its purpose.\", \"example\": \"All production web server hosts across US-East region.\"},\n    \"organization\": {\"type\": \"integer\", \"description\": \"ID of the organization that owns this inventory.\", \"example\": 1},\n    \"kind\"\
  : {\"type\": \"string\", \"enum\": [\"\", \"smart\", \"constructed\"], \"description\": \"Inventory kind — empty for standard, smart, or constructed.\", \"example\": \"\"},\n    \"host_filter\": {\"type\": \"string\", \"description\": \"Filter expression for smart inventories.\", \"example\": \"\"},\n    \"variables\": {\"type\": \"string\", \"description\": \"Inventory-level variables as a JSON or YAML string.\", \"example\": \"{\\\"ansible_user\\\": \\\"deploy\\\"}\"},\n    \"total_hosts\": {\"type\": \"integer\", \"description\": \"Total number of hosts in this inventory.\", \"example\": 24},\n    \"hosts_with_active_failures\": {\"type\": \"integer\", \"description\": \"Number of hosts with active failures.\", \"example\": 0},\n    \"total_groups\": {\"type\": \"integer\", \"description\": \"Total number of groups in this inventory.\", \"example\": 4},\n    \"has_inventory_sources\": {\"type\": \"boolean\", \"description\": \"Whether this inventory has external inventory sources.\"\
  , \"example\": false},\n    \"created\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"Timestamp when the inventory was created.\", \"example\": \"2026-01-01T00:00:00Z\"},\n    \"modified\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"Timestamp when the inventory was last modified.\", \"example\": \"2026-04-19T00:00:00Z\"}\n  },\n  \"required\": [\"id\", \"name\", \"organization\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/json-schema/ansible-playbooks-inventory-schema.json
tags:
- Ansible
- Automation
- Configuration Management
- DevOps
- Infrastructure As Code
- Orchestration
- Playbooks
title: Inventory
---
