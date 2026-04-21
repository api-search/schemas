---
description: Result of sending a message
layout: schema
name: SendResult
properties_list:
- description: Message identifier
  name: msgId
  type: string
- description: Physical offset message ID
  name: offsetMsgId
  type: string
- description: Queue offset of the message
  name: queueOffset
  type: integer
- description: Queue ID the message was sent to
  name: queueId
  type: integer
- description: ''
  name: sendStatus
  type: string
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-send-result-schema.json
slug: apache-rocketmq-send-result
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: SendResult
---
