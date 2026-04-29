---
description: An Apache Druid data ingestion task for batch or streaming data loading.
layout: schema
name: IngestionTask
properties_list:
- description: Unique task ID assigned by Druid.
  name: id
  type: string
- description: Task type identifier.
  name: type
  type: string
- description: Target datasource name.
  name: dataSource
  type: string
- description: Task group ID for parallel tasks.
  name: groupId
  type: string
- description: Current task status.
  name: status
  type: string
- description: Task creation timestamp.
  name: createdTime
  type: string
- description: Task queue insertion timestamp.
  name: queueInsertionTime
  type: string
- description: Host and port where this task is running.
  name: location
  type: object
- description: Task duration in milliseconds (-1 if still running).
  name: duration
  type: integer
provider_name: Apache Druid
provider_slug: apache-druid
schema_file: json-schema/apache-druid-ingestion-task-schema.json
slug: apache-druid-ingestion-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-druid/refs/heads/main/json-schema/apache-druid-ingestion-task-schema.json\",\n  \"title\": \"IngestionTask\",\n  \"description\": \"An Apache Druid data ingestion task for batch or streaming data loading.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique task ID assigned by Druid.\",\n      \"example\": \"index_kafka_wikipedia_abc123_0\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Task type identifier.\",\n      \"enum\": [\n        \"index\",\n        \"index_parallel\",\n        \"index_kafka\",\n        \"index_kinesis\",\n        \"compact\",\n        \"kill\"\n      ],\n      \"example\": \"index_parallel\"\n    },\n    \"dataSource\": {\n      \"type\": \"string\",\n      \"description\": \"Target datasource name.\",\n   \
  \   \"example\": \"wikipedia\"\n    },\n    \"groupId\": {\n      \"type\": \"string\",\n      \"description\": \"Task group ID for parallel tasks.\",\n      \"example\": \"index_parallel_wikipedia_abc123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current task status.\",\n      \"enum\": [\n        \"WAITING\",\n        \"PENDING\",\n        \"RUNNING\",\n        \"SUCCESS\",\n        \"FAILED\"\n      ],\n      \"example\": \"RUNNING\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Task creation timestamp.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"queueInsertionTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Task queue insertion timestamp.\",\n      \"example\": \"2025-03-15T14:30:05Z\"\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"description\": \"Host and port where this task is\
  \ running.\",\n      \"properties\": {\n        \"host\": {\n          \"type\": \"string\",\n          \"example\": \"druid-worker-01\"\n        },\n        \"port\": {\n          \"type\": \"integer\",\n          \"example\": 8100\n        }\n      }\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Task duration in milliseconds (-1 if still running).\",\n      \"example\": -1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-druid/refs/heads/main/json-schema/apache-druid-ingestion-task-schema.json
tags:
- Analytics
- Apache
- Database
- Kafka
- OLAP
- Open Source
- Real-Time
- SQL
- Time Series
title: IngestionTask
---
