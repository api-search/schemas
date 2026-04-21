---
description: RocketMQ topic
layout: schema
name: Topic
properties_list:
- description: Topic name
  name: name
  type: string
- description: Cluster name
  name: clusterName
  type: string
- description: Number of message queues
  name: queueNum
  type: integer
- description: Permission flags (2=write, 4=read, 6=read+write)
  name: perm
  type: integer
- description: ''
  name: topicFilterType
  type: string
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-topic-schema.json
slug: apache-rocketmq-topic
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: Topic
---
