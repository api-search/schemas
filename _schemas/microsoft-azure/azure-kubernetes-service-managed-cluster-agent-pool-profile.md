---
description: Profile for the container service agent pool.
layout: schema
name: ManagedClusterAgentPoolProfile
properties_list:
- description: Unique name of the agent pool profile in the context of the subscription and resource group.
  name: name
  type: string
- description: Number of agents (VMs) to host docker containers.
  name: count
  type: integer
- description: The size of the agent VMs.
  name: vmSize
  type: string
- description: OS disk size in GB for the agent pool VMs.
  name: osDiskSizeGB
  type: integer
- description: The OS disk type to be used for machines in the agent pool.
  name: osDiskType
  type: string
- description: The operating system type.
  name: osType
  type: string
- description: Specifies the OS SKU.
  name: osSKU
  type: string
- description: The maximum number of pods that can run on a node.
  name: maxPods
  type: integer
- description: The mode of an agent pool.
  name: mode
  type: string
- description: The type of agent pool.
  name: type
  type: string
- description: The list of availability zones to use for nodes (e.g., ["1", "2", "3"]).
  name: availabilityZones
  type: array
- description: Whether to enable auto-scaler.
  name: enableAutoScaling
  type: boolean
- description: The minimum number of nodes for auto-scaling.
  name: minCount
  type: integer
- description: The maximum number of nodes for auto-scaling.
  name: maxCount
  type: integer
- description: The node labels to be persisted across all nodes in the agent pool.
  name: nodeLabels
  type: object
- description: The taints added to new nodes during node pool create and scale.
  name: nodeTaints
  type: array
- description: Settings for upgrading the agentpool.
  name: upgradeSettings
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-kubernetes-service-managed-cluster-agent-pool-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-agent-pool-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterAgentPoolProfile\",\n  \"type\": \"object\",\n  \"description\": \"Profile for the container service agent pool.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the agent pool profile in the context of the subscription and resource group.\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of agents (VMs) to host docker containers.\"\n    },\n    \"vmSize\": {\n      \"type\": \"string\",\n      \"description\": \"The size of the agent VMs.\"\n    },\n    \"osDiskSizeGB\": {\n      \"type\": \"integer\",\n      \"description\": \"OS disk size in GB for the agent pool VMs.\"\n    },\n    \"osDiskType\": {\n      \"type\": \"string\",\n      \"description\": \"The OS disk type to be used for machines in the agent pool.\"\n    },\n    \"osType\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"The operating system type.\"\n    },\n    \"osSKU\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the OS SKU.\"\n    },\n    \"maxPods\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of pods that can run on a node.\"\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"The mode of an agent pool.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of agent pool.\"\n    },\n    \"availabilityZones\": {\n      \"type\": \"array\",\n      \"description\": \"The list of availability zones to use for nodes (e.g., [\\\"1\\\", \\\"2\\\", \\\"3\\\"]).\"\n    },\n    \"enableAutoScaling\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable auto-scaler.\"\n    },\n    \"minCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The minimum number of nodes for auto-scaling.\"\n    },\n    \"maxCount\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"The maximum number of nodes for auto-scaling.\"\n    },\n    \"nodeLabels\": {\n      \"type\": \"object\",\n      \"description\": \"The node labels to be persisted across all nodes in the agent pool.\"\n    },\n    \"nodeTaints\": {\n      \"type\": \"array\",\n      \"description\": \"The taints added to new nodes during node pool create and scale.\"\n    },\n    \"upgradeSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Settings for upgrading the agentpool.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-agent-pool-profile-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ManagedClusterAgentPoolProfile
---
