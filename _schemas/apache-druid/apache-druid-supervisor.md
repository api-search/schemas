---
description: An Apache Druid supervisor for managing continuous streaming data ingestion from Kafka or Kinesis.
layout: schema
name: Supervisor
properties_list:
- description: Supervisor ID (same as datasource name by convention).
  name: id
  type: string
- description: Supervisor operational state.
  name: state
  type: string
- description: Supervisor health status.
  name: healthStatus
  type: string
- description: Detailed supervisor sub-state.
  name: detailedState
  type: string
- description: Full supervisor spec including ioConfig and tuningConfig.
  name: spec
  type: object
- description: When the last task completed.
  name: lastTaskCompletionTime
  type: string
- description: Number of currently active ingestion tasks.
  name: activeTasks
  type: integer
- description: Number of tasks publishing segments.
  name: publishingTasks
  type: integer
provider_name: Apache Druid
provider_slug: apache-druid
schema_file: json-schema/apache-druid-supervisor-schema.json
slug: apache-druid-supervisor
source_filename: apache-druid-supervisor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-druid/refs/heads/main/json-schema/apache-druid-supervisor-schema.json\",\n  \"title\": \"Supervisor\",\n  \"description\": \"An Apache Druid supervisor for managing continuous streaming data ingestion from Kafka or Kinesis.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Supervisor ID (same as datasource name by convention).\",\n      \"example\": \"wikipedia-kafka\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Supervisor operational state.\",\n      \"enum\": [\n        \"PENDING\",\n        \"RUNNING\",\n        \"STOPPING\",\n        \"STOPPED\",\n        \"UNHEALTHY_SUPERVISOR\",\n        \"UNHEALTHY_TASKS\"\n      ],\n      \"example\": \"RUNNING\"\n    },\n    \"healthStatus\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Supervisor health status.\",\n      \"enum\": [\n        \"HEALTHY\",\n        \"UNHEALTHY\"\n      ],\n      \"example\": \"HEALTHY\"\n    },\n    \"detailedState\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed supervisor sub-state.\",\n      \"example\": \"RUNNING\"\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"description\": \"Full supervisor spec including ioConfig and tuningConfig.\"\n    },\n    \"lastTaskCompletionTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the last task completed.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"activeTasks\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of currently active ingestion tasks.\",\n      \"example\": 2\n    },\n    \"publishingTasks\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of tasks publishing segments.\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-druid/refs/heads/main/json-schema/apache-druid-supervisor-schema.json
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
title: Supervisor
---
