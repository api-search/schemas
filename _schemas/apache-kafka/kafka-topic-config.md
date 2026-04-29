---
description: Schema for Apache Kafka topic configuration properties.
layout: schema
name: Kafka Topic Configuration
properties_list:
- description: The name of the topic
  name: topic_name
  type: string
- description: Number of partitions for the topic
  name: partitions_count
  type: integer
- description: The replication factor for the topic
  name: replication_factor
  type: integer
- description: Topic-level configuration overrides
  name: configs
  type: object
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-topic-config.json
slug: kafka-topic-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/apache-kafka/kafka-topic-config.json\",\n  \"title\": \"Kafka Topic Configuration\",\n  \"description\": \"Schema for Apache Kafka topic configuration properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topic_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the topic\"\n    },\n    \"partitions_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Number of partitions for the topic\"\n    },\n    \"replication_factor\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"The replication factor for the topic\"\n    },\n    \"configs\": {\n      \"type\": \"object\",\n      \"description\": \"Topic-level configuration overrides\",\n      \"properties\": {\n        \"cleanup.policy\": {\n          \"type\": \"string\",\n          \"enum\": [\"delete\", \"\
  compact\", \"delete,compact\"],\n          \"description\": \"Log cleanup policy\"\n        },\n        \"retention.ms\": {\n          \"type\": \"integer\",\n          \"description\": \"Retention time in milliseconds\"\n        },\n        \"retention.bytes\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum size a partition can grow to before old log segments are discarded\"\n        },\n        \"segment.bytes\": {\n          \"type\": \"integer\",\n          \"description\": \"Segment file size for the log\"\n        },\n        \"max.message.bytes\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum size of a message that can be appended to the log\"\n        },\n        \"min.insync.replicas\": {\n          \"type\": \"integer\",\n          \"description\": \"Minimum number of replicas that must acknowledge a write\"\n        },\n        \"compression.type\": {\n          \"type\": \"string\",\n          \"enum\": [\"uncompressed\"\
  , \"zstd\", \"lz4\", \"snappy\", \"gzip\", \"producer\"],\n          \"description\": \"Compression codec for the topic\"\n        }\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\"topic_name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-topic-config.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: Kafka Topic Configuration
---
