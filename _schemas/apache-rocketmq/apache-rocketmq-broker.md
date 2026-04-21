---
description: RocketMQ broker
layout: schema
name: Broker
properties_list:
- description: Broker name
  name: brokerName
  type: string
- description: Cluster identifier
  name: clusterId
  type: string
- description: Broker ID (0=master, >0=slave)
  name: brokerId
  type: integer
- description: Broker address (host:port)
  name: brokerAddr
  type: string
- description: Broker version
  name: version
  type: string
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-broker-schema.json
slug: apache-rocketmq-broker
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: Broker
---
