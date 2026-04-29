---
description: Represents a machine pool within a cluster, defining a group of compute nodes with shared configuration.
layout: schema
name: MachinePool
properties_list:
- description: The unique identifier of the machine pool.
  name: id
  type: string
- description: The cloud provider instance type for nodes in this pool.
  name: instance_type
  type: string
- description: The fixed number of nodes in this machine pool.
  name: replicas
  type: integer
- description: Autoscaling configuration for the machine pool.
  name: autoscaling
  type: object
- description: The availability zones where nodes will be placed.
  name: availability_zones
  type: array
- description: Kubernetes labels applied to nodes in this pool.
  name: labels
  type: object
- description: Kubernetes taints applied to nodes in this pool.
  name: taints
  type: array
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-openshift-cluster-manager-machine-pool-schema.json
slug: red-hat-openshift-cluster-manager-machine-pool
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MachinePool\",\n  \"type\": \"object\",\n  \"description\": \"Represents a machine pool within a cluster, defining a group of compute nodes with shared configuration.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the machine pool.\"\n    },\n    \"instance_type\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider instance type for nodes in this pool.\"\n    },\n    \"replicas\": {\n      \"type\": \"integer\",\n      \"description\": \"The fixed number of nodes in this machine pool.\"\n    },\n    \"autoscaling\": {\n      \"type\": \"object\",\n      \"description\": \"Autoscaling configuration for the machine pool.\"\n    },\n    \"availability_zones\": {\n      \"type\": \"array\",\n      \"description\": \"The availability zones where nodes will be placed.\"\n    },\n    \"labels\": {\n   \
  \   \"type\": \"object\",\n      \"description\": \"Kubernetes labels applied to nodes in this pool.\"\n    },\n    \"taints\": {\n      \"type\": \"array\",\n      \"description\": \"Kubernetes taints applied to nodes in this pool.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-openshift-cluster-manager-machine-pool-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: MachinePool
---
