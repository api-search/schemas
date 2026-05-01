---
description: Represents a GKE cluster resource, including its configuration, status, networking, and node pool settings.
layout: schema
name: Google Kubernetes Engine Cluster
properties_list:
- description: The name of the cluster.
  name: name
  type: string
- description: An optional description of the cluster.
  name: description
  type: string
- description: The number of nodes to create in this cluster's default node pool.
  name: initialNodeCount
  type: integer
- description: The name of the Google Compute Engine zone or region in which the cluster resides.
  name: location
  type: string
- description: Parameters used in creating the cluster's nodes.
  name: nodeConfig
  type: object
- description: The name of the Google Compute Engine network to which the cluster is connected.
  name: network
  type: string
- description: The name of the Google Compute Engine subnetwork to which the cluster is connected.
  name: subnetwork
  type: string
- description: The IP address range of the container pods in this cluster.
  name: clusterIpv4Cidr
  type: string
- description: The current status of the cluster.
  name: status
  type: string
- description: The IP address of this cluster's master endpoint.
  name: endpoint
  type: string
- description: The current software version of the master endpoint.
  name: currentMasterVersion
  type: string
- description: The current version of the node software components.
  name: currentNodeVersion
  type: string
- description: The time the cluster was created.
  name: createTime
  type: string
- description: Server-defined URL for the resource.
  name: selfLink
  type: string
provider_name: Google Cloud Kubernetes Engine
provider_slug: google-cloud-kubernetes-engine
schema_file: json-schema/gke-cluster.json
slug: gke-cluster
source_filename: gke-cluster.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-search/google-cloud-kubernetes-engine/refs/heads/main/json-schema/gke-cluster.json\",\n  \"title\": \"Google Kubernetes Engine Cluster\",\n  \"description\": \"Represents a GKE cluster resource, including its configuration, status, networking, and node pool settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cluster.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"An optional description of the cluster.\"\n    },\n    \"initialNodeCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of nodes to create in this cluster's default node pool.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Google Compute Engine zone or region in which the cluster resides.\"\
  \n    },\n    \"nodeConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Parameters used in creating the cluster's nodes.\",\n      \"properties\": {\n        \"machineType\": {\n          \"type\": \"string\",\n          \"description\": \"The name of a Google Compute Engine machine type.\"\n        },\n        \"diskSizeGb\": {\n          \"type\": \"integer\",\n          \"description\": \"Size of the disk attached to each node, specified in GB.\"\n        },\n        \"oauthScopes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"The set of Google API scopes available on the nodes.\"\n        },\n        \"imageType\": {\n          \"type\": \"string\",\n          \"description\": \"The image type to use for this node.\"\n        }\n      }\n    },\n    \"network\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Google Compute Engine network to which the\
  \ cluster is connected.\"\n    },\n    \"subnetwork\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Google Compute Engine subnetwork to which the cluster is connected.\"\n    },\n    \"clusterIpv4Cidr\": {\n      \"type\": \"string\",\n      \"description\": \"The IP address range of the container pods in this cluster.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the cluster.\",\n      \"enum\": [\n        \"STATUS_UNSPECIFIED\",\n        \"PROVISIONING\",\n        \"RUNNING\",\n        \"RECONCILING\",\n        \"STOPPING\",\n        \"ERROR\",\n        \"DEGRADED\"\n      ]\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The IP address of this cluster's master endpoint.\"\n    },\n    \"currentMasterVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The current software version of the master endpoint.\"\n    },\n    \"currentNodeVersion\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The current version of the node software components.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the cluster was created.\"\n    },\n    \"selfLink\": {\n      \"type\": \"string\",\n      \"description\": \"Server-defined URL for the resource.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-kubernetes-engine/refs/heads/main/json-schema/gke-cluster.json
tags:
- Compute
- Containers
- GKE
- Google Cloud
- Kubernetes
- Orchestration
title: Google Kubernetes Engine Cluster
---
