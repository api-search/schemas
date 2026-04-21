---
description: Schema for an Apache Kafka record (message) including key, value, headers, and metadata.
layout: schema
name: Kafka Record
properties_list:
- description: The topic the record belongs to
  name: topic
  type: string
- description: The partition within the topic
  name: partition
  type: integer
- description: The offset of the record within the partition
  name: offset
  type: integer
- description: The timestamp of the record in milliseconds since epoch
  name: timestamp
  type: integer
- description: The type of timestamp
  name: timestampType
  type: string
- description: The record key, used for partitioning. Can be any type.
  name: key
  type: object
- description: The record value (message payload). Can be any type.
  name: value
  type: object
- description: Key-value pairs of record headers
  name: headers
  type: object
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-record.json
slug: kafka-record
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: Kafka Record
---
