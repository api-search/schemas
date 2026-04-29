---
description: An Ocean cluster is a serverless Kubernetes infrastructure engine that automatically manages and optimizes cloud infrastructure for containers, handling node provisioning, scaling, and cost optimization.
layout: schema
name: Spot Ocean Cluster
properties_list:
- description: The unique identifier of the Ocean cluster.
  name: id
  type: string
- description: The name of the Ocean cluster.
  name: name
  type: string
- description: The Ocean controller cluster identifier used by the controller pod.
  name: controllerClusterId
  type: string
- description: The cloud provider region where the cluster is deployed.
  name: region
  type: string
- description: The autoscaler configuration for the Ocean cluster.
  name: autoScaler
  type: object
- description: The capacity configuration for the Ocean cluster.
  name: capacity
  type: object
- description: The optimization strategy for the Ocean cluster.
  name: strategy
  type: object
- description: The timestamp when the cluster was created.
  name: createdAt
  type: string
- description: The timestamp when the cluster was last updated.
  name: updatedAt
  type: string
provider_name: Spot
provider_slug: spot
schema_file: json-schema/ocean-cluster.json
slug: ocean-cluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/spot/blob/main/json-schema/ocean-cluster.json\",\n  \"title\": \"Spot Ocean Cluster\",\n  \"description\": \"An Ocean cluster is a serverless Kubernetes infrastructure engine that automatically manages and optimizes cloud infrastructure for containers, handling node provisioning, scaling, and cost optimization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the Ocean cluster.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Ocean cluster.\"\n    },\n    \"controllerClusterId\": {\n      \"type\": \"string\",\n      \"description\": \"The Ocean controller cluster identifier used by the controller pod.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider region where the\
  \ cluster is deployed.\"\n    },\n    \"autoScaler\": {\n      \"type\": \"object\",\n      \"description\": \"The autoscaler configuration for the Ocean cluster.\",\n      \"properties\": {\n        \"isEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the autoscaler is enabled.\"\n        },\n        \"isAutoConfig\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether automatic configuration is enabled.\"\n        },\n        \"cooldown\": {\n          \"type\": \"integer\",\n          \"description\": \"Cooldown period in seconds between scaling actions.\"\n        },\n        \"resourceLimits\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"maxMemoryGib\": {\n              \"type\": \"integer\",\n              \"description\": \"Maximum memory in GiB for the cluster.\"\n            },\n            \"maxVCpu\": {\n              \"type\": \"integer\",\n              \"description\": \"Maximum vCPUs\
  \ for the cluster.\"\n            }\n          }\n        }\n      }\n    },\n    \"capacity\": {\n      \"type\": \"object\",\n      \"description\": \"The capacity configuration for the Ocean cluster.\",\n      \"properties\": {\n        \"target\": {\n          \"type\": \"integer\",\n          \"description\": \"The desired number of instances.\"\n        },\n        \"minimum\": {\n          \"type\": \"integer\",\n          \"description\": \"The minimum number of instances.\"\n        },\n        \"maximum\": {\n          \"type\": \"integer\",\n          \"description\": \"The maximum number of instances.\"\n        }\n      }\n    },\n    \"strategy\": {\n      \"type\": \"object\",\n      \"description\": \"The optimization strategy for the Ocean cluster.\",\n      \"properties\": {\n        \"spotPercentage\": {\n          \"type\": \"integer\",\n          \"description\": \"Percentage of spot instances in the cluster.\"\n        },\n        \"fallbackToOd\": {\n          \"\
  type\": \"boolean\",\n          \"description\": \"Whether to fall back to on-demand when spot is unavailable.\"\n        },\n        \"utilizeReservedInstances\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to utilize reserved instances.\"\n        },\n        \"utilizeCommitments\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to utilize savings plans and commitments.\"\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the cluster was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the cluster was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/ocean-cluster.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: Spot Ocean Cluster
---
