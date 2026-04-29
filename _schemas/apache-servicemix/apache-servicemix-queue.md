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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-queue-schema.json\",\n  \"title\": \"Queue\",\n  \"description\": \"ActiveMQ message queue\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Queue name\"\n    },\n    \"pendingQueueSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of pending messages\"\n    },\n    \"consumerCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of consumers\"\n    },\n    \"enqueueCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Total enqueued messages\"\n    },\n    \"dequeueCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Total dequeued messages\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-queue-schema.json
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
