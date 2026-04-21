---
description: ConsumerGroup schema from Apache kafka
layout: schema
name: ConsumerGroup
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
  name: consumer_group_id
  type: string
- description: ''
  name: is_simple
  type: boolean
- description: ''
  name: partition_assignor
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: coordinator
  type: object
- description: ''
  name: consumers
  type: object
- description: ''
  name: lag_summary
  type: object
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-rest-proxy-consumer-group-schema.json
slug: kafka-rest-proxy-consumer-group
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: ConsumerGroup
---
