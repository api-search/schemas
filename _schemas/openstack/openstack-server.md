---
description: Schema describing a Nova compute server (instance) returned by the OpenStack Compute API.
layout: schema
name: OpenStack Nova Server
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: tenant_id
  type: string
- description: ''
  name: user_id
  type: string
- description: ''
  name: flavor
  type: object
- description: ''
  name: image
  type: object
- description: ''
  name: addresses
  type: object
- description: ''
  name: key_name
  type: string
- description: ''
  name: security_groups
  type: array
- description: ''
  name: metadata
  type: object
- description: ''
  name: created
  type: string
- description: ''
  name: updated
  type: string
- description: ''
  name: OS-EXT-STS:vm_state
  type: string
- description: ''
  name: OS-EXT-STS:task_state
  type:
  - string
  - 'null'
- description: ''
  name: OS-EXT-STS:power_state
  type: integer
- description: ''
  name: OS-EXT-AZ:availability_zone
  type: string
- description: ''
  name: hostId
  type: string
- description: ''
  name: progress
  type: integer
- description: ''
  name: links
  type: array
provider_name: OpenStack
provider_slug: openstack
schema_file: json-schema/openstack-server-schema.json
slug: openstack-server
source_filename: openstack-server-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/json-schema/openstack-server-schema.json\",\n  \"title\": \"OpenStack Nova Server\",\n  \"description\": \"Schema describing a Nova compute server (instance) returned by the OpenStack Compute API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"name\": { \"type\": \"string\" },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\", \"BUILD\", \"DELETED\", \"ERROR\", \"HARD_REBOOT\", \"MIGRATING\",\n        \"PASSWORD\", \"PAUSED\", \"REBOOT\", \"REBUILD\", \"RESCUE\", \"RESIZE\",\n        \"REVERT_RESIZE\", \"SHELVED\", \"SHELVED_OFFLOADED\", \"SHUTOFF\",\n        \"SOFT_DELETED\", \"SUSPENDED\", \"UNKNOWN\", \"VERIFY_RESIZE\"\n      ]\n    },\n    \"tenant_id\": { \"type\": \"string\" },\n    \"user_id\": { \"type\": \"\
  string\" },\n    \"flavor\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"links\": { \"type\": \"array\", \"items\": { \"type\": \"object\" } }\n      }\n    },\n    \"image\": {\n      \"oneOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": { \"type\": \"string\" },\n            \"links\": { \"type\": \"array\", \"items\": { \"type\": \"object\" } }\n          }\n        },\n        { \"type\": \"string\" }\n      ]\n    },\n    \"addresses\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"addr\": { \"type\": \"string\" },\n            \"version\": { \"type\": \"integer\", \"enum\": [4, 6] },\n            \"OS-EXT-IPS:type\": { \"type\": \"string\", \"enum\": [\"fixed\", \"floating\"] },\n            \"OS-EXT-IPS-MAC:mac_addr\"\
  : { \"type\": \"string\" }\n          }\n        }\n      }\n    },\n    \"key_name\": { \"type\": \"string\" },\n    \"security_groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": { \"name\": { \"type\": \"string\" } }\n      }\n    },\n    \"metadata\": { \"type\": \"object\", \"additionalProperties\": { \"type\": \"string\" } },\n    \"created\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"updated\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"OS-EXT-STS:vm_state\": { \"type\": \"string\" },\n    \"OS-EXT-STS:task_state\": { \"type\": [\"string\", \"null\"] },\n    \"OS-EXT-STS:power_state\": { \"type\": \"integer\" },\n    \"OS-EXT-AZ:availability_zone\": { \"type\": \"string\" },\n    \"hostId\": { \"type\": \"string\" },\n    \"progress\": { \"type\": \"integer\" },\n    \"links\": { \"type\": \"array\", \"items\": { \"type\": \"object\" } }\n  },\n  \"required\": [\"id\", \"name\", \"\
  status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/json-schema/openstack-server-schema.json
tags:
- Cloud Platform
- Infrastructure as a Service
- Open Source
- Virtualization
- Linux Foundation
title: OpenStack Nova Server
---
