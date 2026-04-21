---
description: Request to create a RocketMQ topic
layout: schema
name: TopicRequest
properties_list:
- description: Topic name
  name: name
  type: string
- description: Target cluster
  name: clusterName
  type: string
- description: Number of queues (default 8)
  name: queueNum
  type: integer
- description: Permission (6 = read+write)
  name: perm
  type: integer
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-topic-request-schema.json
slug: apache-rocketmq-topic-request
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: TopicRequest
---
