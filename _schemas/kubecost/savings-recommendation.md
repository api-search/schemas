---
description: A savings recommendation for optimizing Kubernetes infrastructure costs, including cluster right-sizing and container request right-sizing suggestions.
layout: schema
name: Kubecost Savings Recommendation
properties_list:
- description: Name of the cluster the recommendation applies to.
  name: clusterName
  type: string
- description: Namespace of the workload (for container-level recommendations).
  name: namespace
  type: string
- description: Kind of controller (e.g. Deployment, StatefulSet).
  name: controllerKind
  type: string
- description: Name of the controller.
  name: controllerName
  type: string
- description: Name of the container (for container-level recommendations).
  name: containerName
  type: string
- description: Current monthly cost rate.
  name: currentMonthlyRate
  type: number
- description: Recommended monthly cost rate after optimization.
  name: recommendedMonthlyRate
  type: number
- description: Estimated monthly savings from the recommendation.
  name: monthlySavings
  type: number
- description: Current number of nodes in the cluster (for cluster-level recommendations).
  name: currentNodeCount
  type: integer
- description: Recommended number of nodes (for cluster-level recommendations).
  name: recommendedNodeCount
  type: integer
- description: Current node instance type (for cluster-level recommendations).
  name: currentNodeType
  type: string
- description: Recommended node instance type (for cluster-level recommendations).
  name: recommendedNodeType
  type: string
- description: Current CPU request (for container-level recommendations).
  name: currentCPURequest
  type: number
- description: Recommended CPU request (for container-level recommendations).
  name: recommendedCPURequest
  type: number
- description: Current RAM request in bytes (for container-level recommendations).
  name: currentRAMBytesRequest
  type: number
- description: Recommended RAM request in bytes (for container-level recommendations).
  name: recommendedRAMBytesRequest
  type: number
provider_name: Kubecost
provider_slug: kubecost
schema_file: json-schema/savings-recommendation.json
slug: savings-recommendation
source_filename: savings-recommendation.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kubecost/blob/main/json-schema/savings-recommendation.json\",\n  \"title\": \"Kubecost Savings Recommendation\",\n  \"description\": \"A savings recommendation for optimizing Kubernetes infrastructure costs, including cluster right-sizing and container request right-sizing suggestions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the cluster the recommendation applies to.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Namespace of the workload (for container-level recommendations).\"\n    },\n    \"controllerKind\": {\n      \"type\": \"string\",\n      \"description\": \"Kind of controller (e.g. Deployment, StatefulSet).\"\n    },\n    \"controllerName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the controller.\"\
  \n    },\n    \"containerName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the container (for container-level recommendations).\"\n    },\n    \"currentMonthlyRate\": {\n      \"type\": \"number\",\n      \"description\": \"Current monthly cost rate.\"\n    },\n    \"recommendedMonthlyRate\": {\n      \"type\": \"number\",\n      \"description\": \"Recommended monthly cost rate after optimization.\"\n    },\n    \"monthlySavings\": {\n      \"type\": \"number\",\n      \"description\": \"Estimated monthly savings from the recommendation.\"\n    },\n    \"currentNodeCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Current number of nodes in the cluster (for cluster-level recommendations).\"\n    },\n    \"recommendedNodeCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Recommended number of nodes (for cluster-level recommendations).\"\n    },\n    \"currentNodeType\": {\n      \"type\": \"string\",\n      \"description\": \"Current\
  \ node instance type (for cluster-level recommendations).\"\n    },\n    \"recommendedNodeType\": {\n      \"type\": \"string\",\n      \"description\": \"Recommended node instance type (for cluster-level recommendations).\"\n    },\n    \"currentCPURequest\": {\n      \"type\": \"number\",\n      \"description\": \"Current CPU request (for container-level recommendations).\"\n    },\n    \"recommendedCPURequest\": {\n      \"type\": \"number\",\n      \"description\": \"Recommended CPU request (for container-level recommendations).\"\n    },\n    \"currentRAMBytesRequest\": {\n      \"type\": \"number\",\n      \"description\": \"Current RAM request in bytes (for container-level recommendations).\"\n    },\n    \"recommendedRAMBytesRequest\": {\n      \"type\": \"number\",\n      \"description\": \"Recommended RAM request in bytes (for container-level recommendations).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/json-schema/savings-recommendation.json
tags:
- Cloud Cost
- Cost Monitoring
- Kubernetes
- Optimization
- Spending
title: Kubecost Savings Recommendation
---
