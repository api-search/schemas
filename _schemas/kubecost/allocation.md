---
description: A cost allocation record for a Kubernetes workload, containing resource usage metrics and associated costs for CPU, GPU, RAM, storage, network, and load balancers over a given time window.
layout: schema
name: Kubecost Allocation
properties_list:
- description: Name of the allocation.
  name: name
  type: string
- description: Kubernetes metadata properties associated with this allocation.
  name: properties
  type: object
- description: The time window for this allocation.
  name: window
  type: object
- description: Start time of the allocation.
  name: start
  type: string
- description: End time of the allocation.
  name: end
  type: string
- description: Number of CPU cores allocated.
  name: cpuCores
  type: number
- description: Average CPU core request over the window.
  name: cpuCoreRequestAverage
  type: number
- description: Average CPU core usage over the window.
  name: cpuCoreUsageAverage
  type: number
- description: Total CPU core-hours consumed.
  name: cpuCoreHours
  type: number
- description: Total cost attributed to CPU usage.
  name: cpuCost
  type: number
- description: Adjustment applied to CPU cost.
  name: cpuCostAdjustment
  type: number
- description: CPU efficiency ratio (usage / request).
  name: cpuEfficiency
  type: number
- description: Number of GPUs allocated.
  name: gpuCount
  type: number
- description: Total GPU-hours consumed.
  name: gpuHours
  type: number
- description: Total cost attributed to GPU usage.
  name: gpuCost
  type: number
- description: Adjustment applied to GPU cost.
  name: gpuCostAdjustment
  type: number
- description: Total network bytes transferred.
  name: networkTransferBytes
  type: number
- description: Total network bytes received.
  name: networkReceiveBytes
  type: number
- description: Total cost attributed to network usage.
  name: networkCost
  type: number
- description: Adjustment applied to network cost.
  name: networkCostAdjustment
  type: number
- description: Total cost attributed to load balancers.
  name: loadBalancerCost
  type: number
- description: Adjustment applied to load balancer cost.
  name: loadBalancerCostAdjustment
  type: number
- description: Persistent volume bytes allocated.
  name: pvBytes
  type: number
- description: Total persistent volume byte-hours consumed.
  name: pvByteHours
  type: number
- description: Total cost attributed to persistent volumes.
  name: pvCost
  type: number
- description: Adjustment applied to persistent volume cost.
  name: pvCostAdjustment
  type: number
- description: RAM bytes allocated.
  name: ramBytes
  type: number
- description: Average RAM byte request over the window.
  name: ramByteRequestAverage
  type: number
- description: Average RAM byte usage over the window.
  name: ramByteUsageAverage
  type: number
- description: Total RAM byte-hours consumed.
  name: ramByteHours
  type: number
- description: Total cost attributed to RAM usage.
  name: ramCost
  type: number
- description: Adjustment applied to RAM cost.
  name: ramCostAdjustment
  type: number
- description: RAM efficiency ratio (usage / request).
  name: ramEfficiency
  type: number
- description: External (out-of-cluster) costs attributed to this allocation.
  name: externalCost
  type: number
- description: Shared costs attributed to this allocation.
  name: sharedCost
  type: number
- description: Total cost for this allocation.
  name: totalCost
  type: number
- description: Overall efficiency ratio across all resources.
  name: totalEfficiency
  type: number
provider_name: Kubecost
provider_slug: kubecost
schema_file: json-schema/allocation.json
slug: allocation
source_filename: allocation.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kubecost/blob/main/json-schema/allocation.json\",\n  \"title\": \"Kubecost Allocation\",\n  \"description\": \"A cost allocation record for a Kubernetes workload, containing resource usage metrics and associated costs for CPU, GPU, RAM, storage, network, and load balancers over a given time window.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the allocation.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Kubernetes metadata properties associated with this allocation.\",\n      \"properties\": {\n        \"cluster\": {\n          \"type\": \"string\",\n          \"description\": \"Cluster name.\"\n        },\n        \"node\": {\n          \"type\": \"string\",\n          \"description\": \"Node name.\"\n        },\n        \"namespace\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Namespace name.\"\n        },\n        \"controller\": {\n          \"type\": \"string\",\n          \"description\": \"Controller name.\"\n        },\n        \"controllerKind\": {\n          \"type\": \"string\",\n          \"description\": \"Kind of controller (e.g. Deployment, StatefulSet, DaemonSet).\"\n        },\n        \"pod\": {\n          \"type\": \"string\",\n          \"description\": \"Pod name.\"\n        },\n        \"container\": {\n          \"type\": \"string\",\n          \"description\": \"Container name.\"\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Kubernetes labels applied to the workload.\"\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n      \
  \    \"description\": \"Kubernetes annotations applied to the workload.\"\n        },\n        \"services\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Kubernetes services associated with the workload.\"\n        }\n      }\n    },\n    \"window\": {\n      \"type\": \"object\",\n      \"description\": \"The time window for this allocation.\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Start of the allocation window.\"\n        },\n        \"end\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"End of the allocation window.\"\n        }\n      }\n    },\n    \"start\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Start time of the allocation.\"\n    },\n    \"end\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"End time of the allocation.\"\n    },\n    \"cpuCores\": {\n      \"type\": \"number\",\n      \"description\": \"Number of CPU cores allocated.\"\n    },\n    \"cpuCoreRequestAverage\": {\n      \"type\": \"number\",\n      \"description\": \"Average CPU core request over the window.\"\n    },\n    \"cpuCoreUsageAverage\": {\n      \"type\": \"number\",\n      \"description\": \"Average CPU core usage over the window.\"\n    },\n    \"cpuCoreHours\": {\n      \"type\": \"number\",\n      \"description\": \"Total CPU core-hours consumed.\"\n    },\n    \"cpuCost\": {\n      \"type\": \"number\",\n      \"description\": \"Total cost attributed to CPU usage.\"\n    },\n    \"cpuCostAdjustment\": {\n      \"type\": \"number\",\n      \"description\": \"Adjustment applied to CPU cost.\"\n    },\n    \"cpuEfficiency\": {\n      \"type\": \"number\",\n      \"description\": \"CPU efficiency ratio (usage / request).\"\n    },\n   \
  \ \"gpuCount\": {\n      \"type\": \"number\",\n      \"description\": \"Number of GPUs allocated.\"\n    },\n    \"gpuHours\": {\n      \"type\": \"number\",\n      \"description\": \"Total GPU-hours consumed.\"\n    },\n    \"gpuCost\": {\n      \"type\": \"number\",\n      \"description\": \"Total cost attributed to GPU usage.\"\n    },\n    \"gpuCostAdjustment\": {\n      \"type\": \"number\",\n      \"description\": \"Adjustment applied to GPU cost.\"\n    },\n    \"networkTransferBytes\": {\n      \"type\": \"number\",\n      \"description\": \"Total network bytes transferred.\"\n    },\n    \"networkReceiveBytes\": {\n      \"type\": \"number\",\n      \"description\": \"Total network bytes received.\"\n    },\n    \"networkCost\": {\n      \"type\": \"number\",\n      \"description\": \"Total cost attributed to network usage.\"\n    },\n    \"networkCostAdjustment\": {\n      \"type\": \"number\",\n      \"description\": \"Adjustment applied to network cost.\"\n    },\n    \"loadBalancerCost\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"Total cost attributed to load balancers.\"\n    },\n    \"loadBalancerCostAdjustment\": {\n      \"type\": \"number\",\n      \"description\": \"Adjustment applied to load balancer cost.\"\n    },\n    \"pvBytes\": {\n      \"type\": \"number\",\n      \"description\": \"Persistent volume bytes allocated.\"\n    },\n    \"pvByteHours\": {\n      \"type\": \"number\",\n      \"description\": \"Total persistent volume byte-hours consumed.\"\n    },\n    \"pvCost\": {\n      \"type\": \"number\",\n      \"description\": \"Total cost attributed to persistent volumes.\"\n    },\n    \"pvCostAdjustment\": {\n      \"type\": \"number\",\n      \"description\": \"Adjustment applied to persistent volume cost.\"\n    },\n    \"ramBytes\": {\n      \"type\": \"number\",\n      \"description\": \"RAM bytes allocated.\"\n    },\n    \"ramByteRequestAverage\": {\n      \"type\": \"number\",\n      \"description\": \"Average RAM byte request\
  \ over the window.\"\n    },\n    \"ramByteUsageAverage\": {\n      \"type\": \"number\",\n      \"description\": \"Average RAM byte usage over the window.\"\n    },\n    \"ramByteHours\": {\n      \"type\": \"number\",\n      \"description\": \"Total RAM byte-hours consumed.\"\n    },\n    \"ramCost\": {\n      \"type\": \"number\",\n      \"description\": \"Total cost attributed to RAM usage.\"\n    },\n    \"ramCostAdjustment\": {\n      \"type\": \"number\",\n      \"description\": \"Adjustment applied to RAM cost.\"\n    },\n    \"ramEfficiency\": {\n      \"type\": \"number\",\n      \"description\": \"RAM efficiency ratio (usage / request).\"\n    },\n    \"externalCost\": {\n      \"type\": \"number\",\n      \"description\": \"External (out-of-cluster) costs attributed to this allocation.\"\n    },\n    \"sharedCost\": {\n      \"type\": \"number\",\n      \"description\": \"Shared costs attributed to this allocation.\"\n    },\n    \"totalCost\": {\n      \"type\": \"number\"\
  ,\n      \"description\": \"Total cost for this allocation.\"\n    },\n    \"totalEfficiency\": {\n      \"type\": \"number\",\n      \"description\": \"Overall efficiency ratio across all resources.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/json-schema/allocation.json
tags:
- Cloud Cost
- Cost Monitoring
- Kubernetes
- Optimization
- Spending
title: Kubecost Allocation
---
