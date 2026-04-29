---
description: A virtual node group (launch specification) defines a set of node configurations within an Ocean cluster, allowing different workloads to run on nodes with specific instance types, labels, and taints.
layout: schema
name: Spot Virtual Node Group
properties_list:
- description: The unique identifier of the virtual node group.
  name: id
  type: string
- description: The name of the virtual node group.
  name: name
  type: string
- description: The identifier of the parent Ocean cluster.
  name: oceanId
  type: string
- description: The AMI or image ID for instances in this virtual node group.
  name: imageId
  type: string
- description: List of allowed instance types for this virtual node group.
  name: instanceTypes
  type: array
- description: Kubernetes labels to apply to nodes in this virtual node group.
  name: labels
  type: array
- description: Kubernetes taints to apply to nodes in this virtual node group.
  name: taints
  type: array
provider_name: Spot
provider_slug: spot
schema_file: json-schema/virtual-node-group.json
slug: virtual-node-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/spot/blob/main/json-schema/virtual-node-group.json\",\n  \"title\": \"Spot Virtual Node Group\",\n  \"description\": \"A virtual node group (launch specification) defines a set of node configurations within an Ocean cluster, allowing different workloads to run on nodes with specific instance types, labels, and taints.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the virtual node group.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the virtual node group.\"\n    },\n    \"oceanId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the parent Ocean cluster.\"\n    },\n    \"imageId\": {\n      \"type\": \"string\",\n      \"description\": \"The AMI or image ID for instances in this virtual node\
  \ group.\"\n    },\n    \"instanceTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of allowed instance types for this virtual node group.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"description\": \"Kubernetes labels to apply to nodes in this virtual node group.\"\n    },\n    \"taints\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          },\n          \"effect\": {\n            \"type\": \"string\",\n            \"enum\": [\"NoSchedule\", \"PreferNoSchedule\"\
  , \"NoExecute\"]\n          }\n        }\n      },\n      \"description\": \"Kubernetes taints to apply to nodes in this virtual node group.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/virtual-node-group.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: Spot Virtual Node Group
---
