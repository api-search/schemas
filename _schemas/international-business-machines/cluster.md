---
description: An IBM Cloud Kubernetes Service cluster.
layout: schema
name: Kubernetes Cluster
properties_list:
- description: The unique identifier of the cluster.
  name: id
  type: string
- description: The name of the cluster.
  name: name
  type: string
- description: The current state of the cluster.
  name: state
  type: string
- description: The data center location.
  name: location
  type: string
- description: The IBM Cloud region.
  name: region
  type: string
- description: The Kubernetes version of the master.
  name: masterKubeVersion
  type: string
- description: The number of worker nodes.
  name: workerCount
  type: integer
- description: The resource group ID.
  name: resourceGroup
  type: string
- description: The infrastructure provider (e.g., vpc-gen2, classic).
  name: provider
  type: string
- description: The cluster type (e.g., kubernetes, openshift).
  name: type
  type: string
- description: The date the cluster was created.
  name: createdDate
  type: string
provider_name: International Business Machines
provider_slug: international-business-machines
schema_file: json-schema/cluster.json
slug: cluster
source_filename: cluster.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"cluster.json\",\n  \"title\": \"Kubernetes Cluster\",\n  \"description\": \"An IBM Cloud Kubernetes Service cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the cluster.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cluster.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the cluster.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The data center location.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The IBM Cloud region.\"\n    },\n    \"masterKubeVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The Kubernetes version of the master.\"\n    },\n    \"workerCount\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"The number of worker nodes.\"\n    },\n    \"resourceGroup\": {\n      \"type\": \"string\",\n      \"description\": \"The resource group ID.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The infrastructure provider (e.g., vpc-gen2, classic).\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The cluster type (e.g., kubernetes, openshift).\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date the cluster was created.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"state\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/json-schema/cluster.json
tags:
- Artificial Intelligence
- Cloud
- Enterprise
- IBM
title: Kubernetes Cluster
---
