---
description: Schema for an Apache Pulsar message including metadata and payload.
layout: schema
name: Apache Pulsar Message
properties_list:
- description: Unique message ID in format ledgerId:entryId:partitionIndex
  name: messageId
  type: string
- description: The message payload, encoded according to the topic schema
  name: payload
  type: object
- description: Message key used for topic compaction and Key_Shared subscriptions
  name: key
  type: string
- description: Ordering key for Key_Shared subscription ordering
  name: orderingKey
  type: string
- description: User-defined key-value properties attached to the message
  name: properties
  type: object
- description: Timestamp when the message was published
  name: publishTime
  type: string
- description: Application-defined event time
  name: eventTime
  type: string
- description: Sequence ID for deduplication
  name: sequenceId
  type: integer
- description: Name of the producer that published the message
  name: producerName
  type: string
- description: Number of times the message has been redelivered
  name: redeliveryCount
  type: integer
- description: Schema version used to encode the message
  name: schemaVersion
  type: string
- description: Full topic name (persistent://tenant/namespace/topic)
  name: topic
  type: string
provider_name: Apache Pulsar
provider_slug: apache-pulsar
schema_file: json-schema/pulsar-message.json
slug: pulsar-message
tags:
- Cloud Native
- Messaging
- Multi-Tenant
- Pub-Sub
- Streaming
- Apache
- Open Source
title: Apache Pulsar Message
---
