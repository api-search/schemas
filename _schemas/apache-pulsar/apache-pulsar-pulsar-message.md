---
description: Schema for an Apache Pulsar message including metadata and payload.
layout: schema
name: PulsarMessage
properties_list:
- description: Unique message ID in format ledgerId:entryId:partitionIndex
  name: messageId
  type: string
- description: The message payload, encoded according to the topic schema
  name: payload
  type: object
- description: Message key used for topic compaction and Key_Shared subscriptions
  name: key
  type: string
- description: Ordering key for Key_Shared subscription ordering
  name: orderingKey
  type: string
- description: User-defined key-value properties attached to the message
  name: properties
  type: object
- description: Timestamp when the message was published
  name: publishTime
  type: string
- description: Application-defined event time
  name: eventTime
  type: string
- description: Sequence ID for deduplication
  name: sequenceId
  type: integer
- description: Name of the producer that published the message
  name: producerName
  type: string
- description: Number of times the message has been redelivered
  name: redeliveryCount
  type: integer
- description: Schema version used to encode the message
  name: schemaVersion
  type: string
- description: Full topic name (persistent://tenant/namespace/topic)
  name: topic
  type: string
provider_name: Apache Pulsar
provider_slug: apache-pulsar
schema_file: json-schema/apache-pulsar-pulsar-message-schema.json
slug: apache-pulsar-pulsar-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pulsar/refs/heads/main/json-schema/apache-pulsar-pulsar-message-schema.json\",\n  \"title\": \"PulsarMessage\",\n  \"description\": \"Schema for an Apache Pulsar message including metadata and payload.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messageId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique message ID in format ledgerId:entryId:partitionIndex\"\n    },\n    \"payload\": {\n      \"description\": \"The message payload, encoded according to the topic schema\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Message key used for topic compaction and Key_Shared subscriptions\"\n    },\n    \"orderingKey\": {\n      \"type\": \"string\",\n      \"description\": \"Ordering key for Key_Shared subscription ordering\"\n    },\n    \"properties\": {\n      \"type\": \"object\"\
  ,\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"User-defined key-value properties attached to the message\"\n    },\n    \"publishTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the message was published\"\n    },\n    \"eventTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Application-defined event time\"\n    },\n    \"sequenceId\": {\n      \"type\": \"integer\",\n      \"description\": \"Sequence ID for deduplication\"\n    },\n    \"producerName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the producer that published the message\"\n    },\n    \"redeliveryCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times the message has been redelivered\"\n    },\n    \"schemaVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Schema version used to encode the\
  \ message\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"Full topic name (persistent://tenant/namespace/topic)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pulsar/refs/heads/main/json-schema/apache-pulsar-pulsar-message-schema.json
tags:
- Cloud Native
- Messaging
- Multi-Tenant
- Pub-Sub
- Streaming
- Apache
- Open Source
title: PulsarMessage
---
