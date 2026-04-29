---
description: Helix cluster configuration and state
layout: schema
name: Cluster
properties_list:
- description: Cluster name
  name: id
  type: string
- description: Active controller node
  name: controller
  type: string
- description: Whether the cluster is paused
  name: paused
  type: boolean
- description: List of disabled instances
  name: disabledInstances
  type: array
- description: List of live instances
  name: liveInstances
  type: array
provider_name: Apache Helix
provider_slug: apache-helix
schema_file: json-schema/helix-rest-cluster-schema.json
slug: helix-rest-cluster
source_filename: helix-rest-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-helix/json-schema/helix-rest-cluster-schema.json\",\n  \"title\": \"Cluster\",\n  \"type\": \"object\",\n  \"description\": \"Helix cluster configuration and state\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster name\",\n      \"example\": \"my-cluster\"\n    },\n    \"controller\": {\n      \"type\": \"string\",\n      \"description\": \"Active controller node\",\n      \"example\": \"controller_host_12345\"\n    },\n    \"paused\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cluster is paused\",\n      \"example\": false\n    },\n    \"disabledInstances\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of disabled instances\"\n    },\n    \"liveInstances\": {\n      \"type\": \"array\",\n      \"items\": {\n\
  \        \"type\": \"string\"\n      },\n      \"description\": \"List of live instances\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-helix/refs/heads/main/json-schema/helix-rest-cluster-schema.json
tags:
- Apache
- Cluster Management
- Distributed Systems
- Open Source
- Partitioning
- Replication
title: Cluster
---
