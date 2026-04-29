---
description: Configuration and state of a Routine Load job that continuously ingests data from Apache Kafka into Doris.
layout: schema
name: RoutineLoadJob
properties_list:
- description: Routine Load job ID.
  name: id
  type: integer
- description: Name of the Routine Load job.
  name: name
  type: string
- description: Target database name.
  name: dbName
  type: string
- description: Target table name.
  name: tableName
  type: string
- description: Current state of the load job.
  name: state
  type: string
- description: Data source type.
  name: dataSourceType
  type: string
- description: Kafka broker list.
  name: kafkaBrokerList
  type: string
- description: Kafka topic to consume from.
  name: kafkaTopic
  type: string
- description: Data format.
  name: format
  type: string
- description: Total number of rows loaded since job start.
  name: totalRows
  type: integer
- description: Number of rows successfully loaded.
  name: loadedRows
  type: integer
- description: Number of rows filtered.
  name: filteredRows
  type: integer
- description: Job creation time.
  name: createTime
  type: string
provider_name: Apache Doris
provider_slug: apache-doris
schema_file: json-schema/apache-doris-routine-load-job-schema.json
slug: apache-doris-routine-load-job
source_filename: apache-doris-routine-load-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-doris/refs/heads/main/json-schema/apache-doris-routine-load-job-schema.json\",\n  \"title\": \"RoutineLoadJob\",\n  \"description\": \"Configuration and state of a Routine Load job that continuously ingests data from Apache Kafka into Doris.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Routine Load job ID.\",\n      \"example\": 601\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Routine Load job.\",\n      \"example\": \"kafka-sales-load\"\n    },\n    \"dbName\": {\n      \"type\": \"string\",\n      \"description\": \"Target database name.\",\n      \"example\": \"analytics\"\n    },\n    \"tableName\": {\n      \"type\": \"string\",\n      \"description\": \"Target table name.\",\n      \"example\": \"sales_events\"\n\
  \    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the load job.\",\n      \"enum\": [\n        \"NEED_SCHEDULE\",\n        \"RUNNING\",\n        \"PAUSED\",\n        \"STOPPED\",\n        \"CANCELLED\"\n      ],\n      \"example\": \"RUNNING\"\n    },\n    \"dataSourceType\": {\n      \"type\": \"string\",\n      \"description\": \"Data source type.\",\n      \"enum\": [\n        \"KAFKA\"\n      ],\n      \"example\": \"KAFKA\"\n    },\n    \"kafkaBrokerList\": {\n      \"type\": \"string\",\n      \"description\": \"Kafka broker list.\",\n      \"example\": \"broker1:9092,broker2:9092\"\n    },\n    \"kafkaTopic\": {\n      \"type\": \"string\",\n      \"description\": \"Kafka topic to consume from.\",\n      \"example\": \"sales-events\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"Data format.\",\n      \"enum\": [\n        \"CSV\",\n        \"JSON\",\n        \"AVRO\"\n      ],\n      \"example\"\
  : \"JSON\"\n    },\n    \"totalRows\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of rows loaded since job start.\",\n      \"example\": 5000000\n    },\n    \"loadedRows\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows successfully loaded.\",\n      \"example\": 4999800\n    },\n    \"filteredRows\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows filtered.\",\n      \"example\": 200\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Job creation time.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"dbName\",\n    \"tableName\",\n    \"kafkaBrokerList\",\n    \"kafkaTopic\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-doris/refs/heads/main/json-schema/apache-doris-routine-load-job-schema.json
tags:
- Analytics
- Apache
- Database
- Lakehouse
- MPP
- OLAP
- Open Source
- Real-Time
- SQL
title: RoutineLoadJob
---
