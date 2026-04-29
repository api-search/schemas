---
description: Stream partition assigned to a task
layout: schema
name: Partition
properties_list:
- description: System name (e.g. kafka)
  name: systemName
  type: string
- description: Stream/topic name
  name: stream
  type: string
- description: Partition number
  name: partitionId
  type: integer
provider_name: Apache Samza
provider_slug: apache-samza
schema_file: json-schema/apache-samza-partition-schema.json
slug: apache-samza-partition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-partition-schema.json\",\n  \"title\": \"Partition\",\n  \"description\": \"Stream partition assigned to a task\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"systemName\": {\n      \"type\": \"string\",\n      \"description\": \"System name (e.g. kafka)\"\n    },\n    \"stream\": {\n      \"type\": \"string\",\n      \"description\": \"Stream/topic name\"\n    },\n    \"partitionId\": {\n      \"type\": \"integer\",\n      \"description\": \"Partition number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-partition-schema.json
tags:
- Big Data
- Hadoop
- Kafka
- Stream Processing
- Streaming
- Apache
- Open Source
title: Partition
---
