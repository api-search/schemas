---
description: Parameters to be applied to the cluster-autoscaler.
layout: schema
name: ManagedClusterAutoScalerProfile
properties_list:
- description: Detects similar node pools and balances the number of nodes between them.
  name: balance-similar-node-groups
  type: string
- description: If set to true, all daemonset pods on empty nodes will be evicted before deletion of the node.
  name: daemonset-eviction-for-empty-nodes
  type: boolean
- description: If set to true, all daemonset pods on occupied nodes will be evicted before deletion of the node.
  name: daemonset-eviction-for-occupied-nodes
  type: boolean
- description: The expander to use when scaling up.
  name: expander
  type: string
- description: The maximum number of empty nodes that can be deleted at the same time.
  name: max-empty-bulk-delete
  type: string
- description: Maximum number of seconds the cluster autoscaler waits for pod termination when trying to scale down a node.
  name: max-graceful-termination-sec
  type: string
- description: The maximum time the autoscaler waits for a node to be provisioned.
  name: max-node-provision-time
  type: string
- description: Maximum percentage of unready nodes in the cluster. After this percentage is exceeded, the cluster autoscaler halts operations.
  name: max-total-unready-percentage
  type: string
- description: For scenarios like burst/batch scale where you do not want CA to act before the kubernetes scheduler could schedule all the pods.
  name: new-pod-scale-up-delay
  type: string
- description: Number of allowed unready nodes, irrespective of max-total-unready-percentage.
  name: ok-total-unready-count
  type: string
- description: How often the cluster is reevaluated for scale up or down.
  name: scan-interval
  type: string
- description: How long after scale up that scale down evaluation resumes.
  name: scale-down-delay-after-add
  type: string
- description: How long after node deletion that scale down evaluation resumes.
  name: scale-down-delay-after-delete
  type: string
- description: How long after scale down failure that scale down evaluation resumes.
  name: scale-down-delay-after-failure
  type: string
- description: How long a node should be unneeded before it is eligible for scale down.
  name: scale-down-unneeded-time
  type: string
- description: How long an unready node should be unneeded before it is eligible for scale down.
  name: scale-down-unready-time
  type: string
- description: Node utilization level, defined as sum of requested resources divided by capacity, below which a node can be considered for scale down.
  name: scale-down-utilization-threshold
  type: string
- description: Whether the cluster autoscaler will skip deleting nodes with pods with local storage.
  name: skip-nodes-with-local-storage
  type: string
- description: Whether the cluster autoscaler will skip deleting nodes with pods from kube-system (except for DaemonSet or mirror pods).
  name: skip-nodes-with-system-pods
  type: string
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-auto-scaler-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-auto-scaler-profile
source_filename: azure-kubernetes-service-managed-cluster-auto-scaler-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterAutoScalerProfile\",\n  \"type\": \"object\",\n  \"description\": \"Parameters to be applied to the cluster-autoscaler.\",\n  \"properties\": {\n    \"balance-similar-node-groups\": {\n      \"type\": \"string\",\n      \"description\": \"Detects similar node pools and balances the number of nodes between them.\"\n    },\n    \"daemonset-eviction-for-empty-nodes\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to true, all daemonset pods on empty nodes will be evicted before deletion of the node.\"\n    },\n    \"daemonset-eviction-for-occupied-nodes\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to true, all daemonset pods on occupied nodes will be evicted before deletion of the node.\"\n    },\n    \"expander\": {\n      \"type\": \"string\",\n      \"description\": \"The expander to use when scaling up.\"\n    },\n    \"max-empty-bulk-delete\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The maximum number of empty nodes that can be deleted at the same time.\"\n    },\n    \"max-graceful-termination-sec\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum number of seconds the cluster autoscaler waits for pod termination when trying to scale down a node.\"\n    },\n    \"max-node-provision-time\": {\n      \"type\": \"string\",\n      \"description\": \"The maximum time the autoscaler waits for a node to be provisioned.\"\n    },\n    \"max-total-unready-percentage\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum percentage of unready nodes in the cluster. After this percentage is exceeded, the cluster autoscaler halts operations.\"\n    },\n    \"new-pod-scale-up-delay\": {\n      \"type\": \"string\",\n      \"description\": \"For scenarios like burst/batch scale where you do not want CA to act before the kubernetes scheduler could schedule all the pods.\"\n    },\n    \"ok-total-unready-count\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Number of allowed unready nodes, irrespective of max-total-unready-percentage.\"\n    },\n    \"scan-interval\": {\n      \"type\": \"string\",\n      \"description\": \"How often the cluster is reevaluated for scale up or down.\"\n    },\n    \"scale-down-delay-after-add\": {\n      \"type\": \"string\",\n      \"description\": \"How long after scale up that scale down evaluation resumes.\"\n    },\n    \"scale-down-delay-after-delete\": {\n      \"type\": \"string\",\n      \"description\": \"How long after node deletion that scale down evaluation resumes.\"\n    },\n    \"scale-down-delay-after-failure\": {\n      \"type\": \"string\",\n      \"description\": \"How long after scale down failure that scale down evaluation resumes.\"\n    },\n    \"scale-down-unneeded-time\": {\n      \"type\": \"string\",\n      \"description\": \"How long a node should be unneeded before it is eligible for scale down.\"\n    },\n    \"scale-down-unready-time\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"How long an unready node should be unneeded before it is eligible for scale down.\"\n    },\n    \"scale-down-utilization-threshold\": {\n      \"type\": \"string\",\n      \"description\": \"Node utilization level, defined as sum of requested resources divided by capacity, below which a node can be considered for scale down.\"\n    },\n    \"skip-nodes-with-local-storage\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the cluster autoscaler will skip deleting nodes with pods with local storage.\"\n    },\n    \"skip-nodes-with-system-pods\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the cluster autoscaler will skip deleting nodes with pods from kube-system (except for DaemonSet or mirror pods).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-auto-scaler-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterAutoScalerProfile
---
