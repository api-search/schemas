---
description: A Cluster represents a connected Kubernetes cluster with the Camel Bridge operator installed, serving as a deployment target for integrations.
layout: schema
name: Jetic Cluster
properties_list:
- description: Unique cluster identifier.
  name: id
  type: string
- description: Name of the cluster.
  name: name
  type: string
- description: Cloud provider or infrastructure type.
  name: provider
  type: string
- description: Cluster region.
  name: region
  type: string
- description: Status of the Camel Bridge operator on this cluster.
  name: camelBridgeStatus
  type: string
- description: Kubernetes version running on the cluster.
  name: kubernetesVersion
  type: string
- description: Number of active deployments on this cluster.
  name: deploymentCount
  type: integer
- description: Timestamp when the cluster was registered.
  name: createdAt
  type: string
provider_name: Jetic
provider_slug: jetic
schema_file: json-schema/cluster.json
slug: cluster
source_filename: cluster.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/jetic/blob/main/json-schema/cluster.json\",\n  \"title\": \"Jetic Cluster\",\n  \"description\": \"A Cluster represents a connected Kubernetes cluster with the Camel Bridge operator installed, serving as a deployment target for integrations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique cluster identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the cluster.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud provider or infrastructure type.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster region.\"\n    },\n    \"camelBridgeStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"connected\",\n        \"disconnected\",\n        \"error\"\
  \n      ],\n      \"description\": \"Status of the Camel Bridge operator on this cluster.\"\n    },\n    \"kubernetesVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes version running on the cluster.\"\n    },\n    \"deploymentCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active deployments on this cluster.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the cluster was registered.\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/json-schema/cluster.json
tags:
- Apache Camel
- Integrations
- iPaaS
- Pro-Code API Composition
title: Jetic Cluster
---
