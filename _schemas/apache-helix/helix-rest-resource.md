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
tags:
- Apache
- Cluster Management
- Distributed Systems
- Open Source
- Partitioning
- Replication
title: Resource
---
