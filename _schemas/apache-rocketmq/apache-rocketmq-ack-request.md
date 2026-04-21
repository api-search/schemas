---
description: Request to acknowledge a message
layout: schema
name: AckRequest
properties_list:
- description: Receipt handle from receive response
  name: receiptHandle
  type: string
- description: Topic name
  name: topic
  type: string
- description: Consumer group
  name: consumerGroup
  type: string
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-ack-request-schema.json
slug: apache-rocketmq-ack-request
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: AckRequest
---
