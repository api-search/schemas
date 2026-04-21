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
