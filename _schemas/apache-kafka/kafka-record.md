---
description: Schema for an Apache Kafka record (message) including key, value, headers, and metadata.
layout: schema
name: Kafka Record
properties_list:
- description: The topic the record belongs to
  name: topic
  type: string
- description: The partition within the topic
  name: partition
  type: integer
- description: The offset of the record within the partition
  name: offset
  type: integer
- description: The timestamp of the record in milliseconds since epoch
  name: timestamp
  type: integer
- description: The type of timestamp
  name: timestampType
  type: string
- description: The record key, used for partitioning. Can be any type.
  name: key
  type: object
- description: The record value (message payload). Can be any type.
  name: value
  type: object
- description: Key-value pairs of record headers
  name: headers
  type: object
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-record.json
slug: kafka-record
source_filename: kafka-record.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/apache-kafka/kafka-record.json\",\n  \"title\": \"Kafka Record\",\n  \"description\": \"Schema for an Apache Kafka record (message) including key, value, headers, and metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"The topic the record belongs to\"\n    },\n    \"partition\": {\n      \"type\": \"integer\",\n      \"description\": \"The partition within the topic\"\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"The offset of the record within the partition\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"The timestamp of the record in milliseconds since epoch\"\n    },\n    \"timestampType\": {\n      \"type\": \"string\",\n      \"enum\": [\"CREATE_TIME\", \"LOG_APPEND_TIME\", \"NO_TIMESTAMP_TYPE\"],\n\
  \      \"description\": \"The type of timestamp\"\n    },\n    \"key\": {\n      \"description\": \"The record key, used for partitioning. Can be any type.\"\n    },\n    \"value\": {\n      \"description\": \"The record value (message payload). Can be any type.\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs of record headers\"\n    }\n  },\n  \"required\": [\"topic\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-record.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: Kafka Record
---
