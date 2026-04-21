---
description: Schema for Apache Kafka topic configuration properties.
layout: schema
name: Kafka Topic Configuration
properties_list:
- description: The name of the topic
  name: topic_name
  type: string
- description: Number of partitions for the topic
  name: partitions_count
  type: integer
- description: The replication factor for the topic
  name: replication_factor
  type: integer
- description: Topic-level configuration overrides
  name: configs
  type: object
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-topic-config.json
slug: kafka-topic-config
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: Kafka Topic Configuration
---
