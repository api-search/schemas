---
description: TopicStats schema from Apache Pulsar
layout: schema
name: TopicStats
properties_list:
- description: ''
  name: msgRateIn
  type: number
- description: ''
  name: msgRateOut
  type: number
- description: ''
  name: msgThroughputIn
  type: number
- description: ''
  name: msgThroughputOut
  type: number
- description: ''
  name: averageMsgSize
  type: number
- description: ''
  name: storageSize
  type: integer
- description: ''
  name: backlogSize
  type: integer
- description: ''
  name: publishers
  type: array
- description: ''
  name: subscriptions
  type: object
provider_name: Apache Pulsar
provider_slug: apache-pulsar
schema_file: json-schema/apache-pulsar-topic-stats-schema.json
slug: apache-pulsar-topic-stats
tags:
- Cloud Native
- Messaging
- Multi-Tenant
- Pub-Sub
- Streaming
- Apache
- Open Source
title: TopicStats
---
