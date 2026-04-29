---
description: Helix resource (distributed data or service) configuration
layout: schema
name: Resource
properties_list:
- description: Resource name
  name: id
  type: string
- description: State model definition reference
  name: stateModelDefRef
  type: string
- description: Number of partitions
  name: numPartitions
  type: integer
- description: Replication factor
  name: replicas
  type: string
- description: Rebalance strategy
  name: rebalanceMode
  type: string
provider_name: Apache Helix
provider_slug: apache-helix
schema_file: json-schema/helix-rest-resource-schema.json
slug: helix-rest-resource
source_filename: helix-rest-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-helix/json-schema/helix-rest-resource-schema.json\",\n  \"title\": \"Resource\",\n  \"type\": \"object\",\n  \"description\": \"Helix resource (distributed data or service) configuration\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name\",\n      \"example\": \"my-resource\"\n    },\n    \"stateModelDefRef\": {\n      \"type\": \"string\",\n      \"description\": \"State model definition reference\",\n      \"example\": \"MasterSlave\"\n    },\n    \"numPartitions\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of partitions\",\n      \"example\": 16\n    },\n    \"replicas\": {\n      \"type\": \"string\",\n      \"description\": \"Replication factor\",\n      \"example\": \"3\"\n    },\n    \"rebalanceMode\": {\n      \"type\": \"string\",\n      \"description\": \"Rebalance strategy\"\
  ,\n      \"example\": \"FULL_AUTO\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-helix/refs/heads/main/json-schema/helix-rest-resource-schema.json
tags:
- Apache
- Cluster Management
- Distributed Systems
- Open Source
- Partitioning
- Replication
title: Resource
---
