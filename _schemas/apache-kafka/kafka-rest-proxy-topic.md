---
description: Topic schema from Apache kafka
layout: schema
name: Topic
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
  name: is_internal
  type: boolean
- description: ''
  name: replication_factor
  type: integer
- description: ''
  name: partitions_count
  type: integer
- description: ''
  name: partitions
  type: object
- description: ''
  name: configs
  type: object
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-rest-proxy-topic-schema.json
slug: kafka-rest-proxy-topic
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: Topic
---
