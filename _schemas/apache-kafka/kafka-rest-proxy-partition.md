---
description: Partition schema from Apache kafka
layout: schema
name: Partition
properties_list:
- description: ''
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: cluster_id
  type: string
- description: ''
  name: topic_name
  type: string
- description: ''
  name: partition_id
  type: integer
- description: ''
  name: leader
  type: object
- description: ''
  name: replicas
  type: array
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-rest-proxy-partition-schema.json
slug: kafka-rest-proxy-partition
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: Partition
---
