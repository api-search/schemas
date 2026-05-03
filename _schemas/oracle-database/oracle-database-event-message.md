---
description: Represents a message in Oracle Transactional Event Queues (TxEventQ), the Kafka-compatible event streaming system built into Oracle Database.
layout: schema
name: Oracle Transactional Event Queue Message
properties_list:
- description: Message key used for partition assignment and ordering guarantees
  name: key
  type:
  - string
  - 'null'
- description: The message payload content, can be any JSON value
  name: value
  type: object
- description: Optional message headers for metadata and routing
  name: headers
  type: object
- description: Name of the TxEventQ topic
  name: topic
  type: string
- description: Partition number within the topic
  name: partition
  type: integer
- description: Sequential offset of the message within its partition
  name: offset
  type: integer
- description: Timestamp when the message was produced or appended
  name: timestamp
  type: string
- description: Type of timestamp
  name: timestampType
  type: string
provider_name: Oracle Database
provider_slug: oracle-database
schema_file: json-schema/oracle-database-event-message.json
slug: oracle-database-event-message
source_filename: oracle-database-event-message.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://oracle.com/schemas/database/event-message.json\",\n  \"title\": \"Oracle Transactional Event Queue Message\",\n  \"description\": \"Represents a message in Oracle Transactional Event Queues (TxEventQ), the Kafka-compatible event streaming system built into Oracle Database.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Message key used for partition assignment and ordering guarantees\"\n    },\n    \"value\": {\n      \"description\": \"The message payload content, can be any JSON value\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"Optional message headers for metadata and routing\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the TxEventQ topic\"\
  \n    },\n    \"partition\": {\n      \"type\": \"integer\",\n      \"description\": \"Partition number within the topic\",\n      \"minimum\": 0\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Sequential offset of the message within its partition\",\n      \"minimum\": 0\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the message was produced or appended\"\n    },\n    \"timestampType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of timestamp\",\n      \"enum\": [\"CREATE_TIME\", \"LOG_APPEND_TIME\"]\n    }\n  },\n  \"required\": [\"value\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-database/refs/heads/main/json-schema/oracle-database-event-message.json
tags:
- Cloud
- Database
- Enterprise
- Oracle
- REST API
- SQL
title: Oracle Transactional Event Queue Message
---
