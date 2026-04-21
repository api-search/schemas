---
description: Request to receive messages from a topic
layout: schema
name: ReceiveRequest
properties_list:
- description: Topic to consume from
  name: topic
  type: string
- description: Consumer group identifier
  name: consumerGroup
  type: string
- description: Maximum messages to pull
  name: maxMessages
  type: integer
- description: Invisible duration in milliseconds
  name: invisibleDuration
  type: integer
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-receive-request-schema.json
slug: apache-rocketmq-receive-request
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: ReceiveRequest
---
