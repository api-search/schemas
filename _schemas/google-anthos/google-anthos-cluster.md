---
description: Schema for an Anthos on-premises cluster resource representing a Kubernetes cluster running on VMware or bare metal infrastructure.
layout: schema
name: Google Anthos On-Prem Cluster
properties_list:
- description: The resource name of the cluster
  name: name
  type: string
- description: A human-readable description of the cluster
  name: description
  type: string
- description: The Anthos on-prem version for the cluster
  name: onPremVersion
  type: string
- description: The admin cluster this user cluster is managed by
  name: adminClusterMembership
  type: string
- description: Current state of the cluster
  name: state
  type: string
- description: The API server endpoint of the cluster
  name: endpoint
  type: string
- description: Timestamp when the cluster was created
  name: createTime
  type: string
- description: Timestamp when the cluster was last updated
  name: updateTime
  type: string
- description: Control plane node configuration
  name: controlPlaneNode
  type: object
- description: Network configuration for the cluster
  name: networkConfig
  type: object
- description: Node pools in this cluster
  name: nodePools
  type: array
provider_name: Google Anthos
provider_slug: google-anthos
schema_file: json-schema/google-anthos-cluster-schema.json
slug: google-anthos-cluster
source_filename: google-anthos-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/anthos/cluster.json\",\n  \"title\": \"Google Anthos On-Prem Cluster\",\n  \"description\": \"Schema for an Anthos on-premises cluster resource representing a Kubernetes cluster running on VMware or bare metal infrastructure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the cluster\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the cluster\"\n    },\n    \"onPremVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The Anthos on-prem version for the cluster\"\n    },\n    \"adminClusterMembership\": {\n      \"type\": \"string\",\n      \"description\": \"The admin cluster this user cluster is managed by\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Current state of the cluster\",\n      \"enum\": [\"STATE_UNSPECIFIED\", \"PROVISIONING\", \"RUNNING\", \"RECONCILING\", \"STOPPING\", \"ERROR\", \"DEGRADED\"]\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The API server endpoint of the cluster\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the cluster was created\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the cluster was last updated\"\n    },\n    \"controlPlaneNode\": {\n      \"$ref\": \"#/$defs/ControlPlaneNodeConfig\",\n      \"description\": \"Control plane node configuration\"\n    },\n    \"networkConfig\": {\n      \"$ref\": \"#/$defs/NetworkConfig\",\n      \"description\": \"Network configuration for the cluster\"\n    },\n    \"nodePools\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"\
  $ref\": \"#/$defs/NodePool\"\n      },\n      \"description\": \"Node pools in this cluster\"\n    }\n  },\n  \"$defs\": {\n    \"ControlPlaneNodeConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for control plane nodes\",\n      \"properties\": {\n        \"cpus\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of CPUs for each control plane node\",\n          \"minimum\": 1\n        },\n        \"memory\": {\n          \"type\": \"integer\",\n          \"description\": \"Memory in megabytes for each control plane node\",\n          \"minimum\": 1\n        },\n        \"replicas\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of control plane node replicas\",\n          \"minimum\": 1\n        }\n      }\n    },\n    \"NetworkConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Network configuration for the cluster\",\n      \"properties\": {\n        \"serviceAddressCidrBlocks\": {\n  \
  \        \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"CIDR blocks for Kubernetes services\"\n        },\n        \"podAddressCidrBlocks\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"CIDR blocks for Kubernetes pods\"\n        }\n      }\n    },\n    \"NodePool\": {\n      \"type\": \"object\",\n      \"description\": \"A node pool within the cluster\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Resource name of the node pool\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the node pool\"\n        },\n        \"cpus\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of CPUs per node\",\n          \"minimum\": 1\n        },\n        \"memoryMb\": {\n         \
  \ \"type\": \"integer\",\n          \"description\": \"Memory in megabytes per node\",\n          \"minimum\": 1\n        },\n        \"replicas\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of node replicas\",\n          \"minimum\": 0\n        },\n        \"imageType\": {\n          \"type\": \"string\",\n          \"description\": \"OS image type for the nodes\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\"STATE_UNSPECIFIED\", \"PROVISIONING\", \"RUNNING\", \"RECONCILING\", \"STOPPING\", \"ERROR\", \"DEGRADED\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-anthos/refs/heads/main/json-schema/google-anthos-cluster-schema.json
tags:
- Container Platform
- Hybrid Cloud
- Kubernetes
- Multi-Cloud
- On-Premises
- Service Mesh
title: Google Anthos On-Prem Cluster
---
