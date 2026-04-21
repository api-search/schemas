---
description: Samza task within a container
layout: schema
name: Task
properties_list:
- description: Task name
  name: taskName
  type: string
- description: Container the task runs on
  name: containerId
  type: string
- description: Task status
  name: status
  type: string
- description: ''
  name: partitions
  type: array
provider_name: Apache Samza
provider_slug: apache-samza
schema_file: json-schema/apache-samza-task-schema.json
slug: apache-samza-task
tags:
- Big Data
- Hadoop
- Kafka
- Stream Processing
- Streaming
- Apache
- Open Source
title: Task
---
