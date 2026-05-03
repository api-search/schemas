---
description: Schema describing a downstream Kubernetes cluster managed by Rancher.
layout: schema
name: Rancher Cluster
properties_list:
- description: Rancher-assigned cluster identifier (for example, c-m-xxxxxxxx).
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Target Kubernetes version (for example, v1.30.5).
  name: kubernetesVersion
  type: string
- description: Provisioning provider such as rke, rke2, k3s, eks, gke, aks, or imported.
  name: provider
  type: string
- description: ''
  name: driver
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: internal
  type: boolean
provider_name: Rancher
provider_slug: rancher
schema_file: json-schema/rancher-cluster.json
slug: rancher-cluster
source_filename: rancher-cluster.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/rancher/refs/heads/main/json-schema/rancher-cluster.json\",\n  \"title\": \"Rancher Cluster\",\n  \"description\": \"Schema describing a downstream Kubernetes cluster managed by Rancher.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Rancher-assigned cluster identifier (for example, c-m-xxxxxxxx).\" },\n    \"name\": { \"type\": \"string\" },\n    \"description\": { \"type\": \"string\" },\n    \"kubernetesVersion\": { \"type\": \"string\", \"description\": \"Target Kubernetes version (for example, v1.30.5).\" },\n    \"provider\": { \"type\": \"string\", \"description\": \"Provisioning provider such as rke, rke2, k3s, eks, gke, aks, or imported.\" },\n    \"driver\": { \"type\": \"string\" },\n    \"state\": { \"type\": \"string\", \"enum\": [\"provisioning\", \"active\", \"updating\", \"\
  error\", \"removing\"] },\n    \"internal\": { \"type\": \"boolean\" }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rancher/refs/heads/main/json-schema/rancher-cluster.json
tags:
- Cluster Management
- Containers
- Kubernetes
- Multi-Cluster
- Open Source
- SUSE
- Platform Engineering
title: Rancher Cluster
---
