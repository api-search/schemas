---
description: An inventory defines a collection of hosts and groups that automation jobs target for execution.
layout: schema
name: Inventory
properties_list:
- description: The unique identifier of the inventory.
  name: id
  type: integer
- description: The name of the inventory.
  name: name
  type: string
- description: A description of the inventory.
  name: description
  type: string
- description: The ID of the organization this inventory belongs to.
  name: organization
  type: integer
- description: The kind of inventory.
  name: kind
  type: string
- description: The total number of hosts in this inventory.
  name: host_count
  type: integer
- description: The total number of groups in this inventory.
  name: total_groups
  type: integer
- description: Whether this inventory has dynamic sources.
  name: has_inventory_sources
  type: boolean
- description: When the inventory was created.
  name: created
  type: string
- description: When the inventory was last modified.
  name: modified
  type: string
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-ansible-automation-platform-inventory-schema.json
slug: red-hat-ansible-automation-platform-inventory
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Inventory\",\n  \"type\": \"object\",\n  \"description\": \"An inventory defines a collection of hosts and groups that automation jobs target for execution.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the inventory.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the inventory.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the inventory.\"\n    },\n    \"organization\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the organization this inventory belongs to.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The kind of inventory.\"\n    },\n    \"host_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of hosts in this inventory.\"\
  \n    },\n    \"total_groups\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of groups in this inventory.\"\n    },\n    \"has_inventory_sources\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this inventory has dynamic sources.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"When the inventory was created.\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"description\": \"When the inventory was last modified.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-ansible-automation-platform-inventory-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Inventory
---
