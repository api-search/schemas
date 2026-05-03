---
description: Schema describing a Rancher project, which groups namespaces within a cluster for tenancy and policy.
layout: schema
name: Rancher Project
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: clusterId
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: resourceQuota
  type: object
- description: ''
  name: namespaceDefaultResourceQuota
  type: object
provider_name: Rancher
provider_slug: rancher
schema_file: json-schema/rancher-project.json
slug: rancher-project
source_filename: rancher-project.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/rancher/refs/heads/main/json-schema/rancher-project.json\",\n  \"title\": \"Rancher Project\",\n  \"description\": \"Schema describing a Rancher project, which groups namespaces within a cluster for tenancy and policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\" },\n    \"name\": { \"type\": \"string\" },\n    \"clusterId\": { \"type\": \"string\" },\n    \"description\": { \"type\": \"string\" },\n    \"resourceQuota\": { \"type\": \"object\" },\n    \"namespaceDefaultResourceQuota\": { \"type\": \"object\" }\n  },\n  \"required\": [\"name\", \"clusterId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rancher/refs/heads/main/json-schema/rancher-project.json
tags:
- Cluster Management
- Containers
- Kubernetes
- Multi-Cluster
- Open Source
- SUSE
- Platform Engineering
title: Rancher Project
---
