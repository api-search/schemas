---
description: Request to send a message to RocketMQ
layout: schema
name: MessageRequest
properties_list:
- description: Target topic name
  name: topic
  type: string
- description: Message body content
  name: body
  type: string
- description: Message tag for filtering
  name: tag
  type: string
- description: Message keys for lookup
  name: keys
  type: array
- description: User-defined message properties
  name: properties
  type: object
- description: Delay level for scheduled messages (0=no delay)
  name: delayLevel
  type: integer
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-message-request-schema.json
slug: apache-rocketmq-message-request
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: MessageRequest
---
