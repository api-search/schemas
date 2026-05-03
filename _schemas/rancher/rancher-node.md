---
description: Schema describing a node registered with a Rancher-managed cluster.
layout: schema
name: Rancher Node
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: clusterId
  type: string
- description: ''
  name: hostname
  type: string
- description: ''
  name: ipAddress
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: roles
  type: array
- description: ''
  name: info
  type: object
provider_name: Rancher
provider_slug: rancher
schema_file: json-schema/rancher-node.json
slug: rancher-node
source_filename: rancher-node.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/rancher/refs/heads/main/json-schema/rancher-node.json\",\n  \"title\": \"Rancher Node\",\n  \"description\": \"Schema describing a node registered with a Rancher-managed cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\" },\n    \"clusterId\": { \"type\": \"string\" },\n    \"hostname\": { \"type\": \"string\" },\n    \"ipAddress\": { \"type\": \"string\" },\n    \"state\": { \"type\": \"string\", \"enum\": [\"registering\", \"active\", \"cordoned\", \"draining\", \"error\", \"removing\"] },\n    \"roles\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\", \"enum\": [\"controlplane\", \"etcd\", \"worker\"] }\n    },\n    \"info\": { \"type\": \"object\" }\n  },\n  \"required\": [\"id\", \"clusterId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rancher/refs/heads/main/json-schema/rancher-node.json
tags:
- Cluster Management
- Containers
- Kubernetes
- Multi-Cluster
- Open Source
- SUSE
- Platform Engineering
title: Rancher Node
---
