---
description: Received RocketMQ message
layout: schema
name: Message
properties_list:
- description: Message identifier
  name: msgId
  type: string
- description: Topic name
  name: topic
  type: string
- description: Message body
  name: body
  type: string
- description: Message tag
  name: tag
  type: string
- description: ''
  name: keys
  type: array
- description: ''
  name: properties
  type: object
- description: Message creation timestamp in milliseconds
  name: bornTimestamp
  type: integer
- description: Handle for acknowledging the message
  name: receiptHandle
  type: string
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-message-schema.json
slug: apache-rocketmq-message
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: Message
---
