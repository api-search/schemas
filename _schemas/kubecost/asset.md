---
description: An individual Kubernetes infrastructure asset such as a node, disk, or load balancer, with associated cost data over a given time window.
layout: schema
name: Kubecost Asset
properties_list:
- description: Type of asset (e.g. Node, Disk, LoadBalancer, ClusterManagement, Network, Attached).
  name: type
  type: string
- description: Metadata properties associated with this asset.
  name: properties
  type: object
- description: The time window for this asset cost record.
  name: window
  type: object
- description: Start time of the asset record.
  name: start
  type: string
- description: End time of the asset record.
  name: end
  type: string
- description: Duration in minutes for the asset record.
  name: minutes
  type: number
- description: Cost adjustment applied to the asset.
  name: adjustment
  type: number
- description: Total cost of the asset over the window.
  name: totalCost
  type: number
provider_name: Kubecost
provider_slug: kubecost
schema_file: json-schema/asset.json
slug: asset
source_filename: asset.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kubecost/blob/main/json-schema/asset.json\",\n  \"title\": \"Kubecost Asset\",\n  \"description\": \"An individual Kubernetes infrastructure asset such as a node, disk, or load balancer, with associated cost data over a given time window.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of asset (e.g. Node, Disk, LoadBalancer, ClusterManagement, Network, Attached).\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata properties associated with this asset.\",\n      \"properties\": {\n        \"cluster\": {\n          \"type\": \"string\",\n          \"description\": \"Cluster name.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Asset name.\"\n        },\n        \"providerID\": {\n         \
  \ \"type\": \"string\",\n          \"description\": \"Cloud provider resource identifier.\"\n        },\n        \"provider\": {\n          \"type\": \"string\",\n          \"description\": \"Cloud provider name (e.g. AWS, Azure, GCP).\"\n        },\n        \"account\": {\n          \"type\": \"string\",\n          \"description\": \"Cloud provider account identifier.\"\n        },\n        \"project\": {\n          \"type\": \"string\",\n          \"description\": \"Cloud provider project identifier.\"\n        },\n        \"service\": {\n          \"type\": \"string\",\n          \"description\": \"Cloud provider service name.\"\n        },\n        \"category\": {\n          \"type\": \"string\",\n          \"description\": \"Asset category.\"\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Labels applied to the asset.\"\n        }\n      }\n    },\n\
  \    \"window\": {\n      \"type\": \"object\",\n      \"description\": \"The time window for this asset cost record.\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Start of the window.\"\n        },\n        \"end\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"End of the window.\"\n        }\n      }\n    },\n    \"start\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Start time of the asset record.\"\n    },\n    \"end\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"End time of the asset record.\"\n    },\n    \"minutes\": {\n      \"type\": \"number\",\n      \"description\": \"Duration in minutes for the asset record.\"\n    },\n    \"adjustment\": {\n      \"type\": \"number\",\n      \"description\": \"Cost adjustment applied to\
  \ the asset.\"\n    },\n    \"totalCost\": {\n      \"type\": \"number\",\n      \"description\": \"Total cost of the asset over the window.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/json-schema/asset.json
tags:
- Cloud Cost
- Cost Monitoring
- Kubernetes
- Optimization
- Spending
title: Kubecost Asset
---
