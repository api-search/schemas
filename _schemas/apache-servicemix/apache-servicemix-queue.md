---
description: ActiveMQ message queue
layout: schema
name: Queue
properties_list:
- description: Queue name
  name: name
  type: string
- description: Number of pending messages
  name: pendingQueueSize
  type: integer
- description: Number of consumers
  name: consumerCount
  type: integer
- description: Total enqueued messages
  name: enqueueCount
  type: integer
- description: Total dequeued messages
  name: dequeueCount
  type: integer
provider_name: Apache ServiceMix
provider_slug: apache-servicemix
schema_file: json-schema/apache-servicemix-queue-schema.json
slug: apache-servicemix-queue
tags:
- Enterprise Integration
- ESB
- Integration
- Messaging
- OSGi
- Apache
- Open Source
title: Queue
---
