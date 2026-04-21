---
description: Samza stream processing job
layout: schema
name: Job
properties_list:
- description: Job name
  name: jobName
  type: string
- description: Job identifier
  name: jobId
  type: string
- description: Current job status
  name: status
  type: string
- description: Number of containers running
  name: containersCount
  type: integer
- description: Total task count
  name: taskCount
  type: integer
provider_name: Apache Samza
provider_slug: apache-samza
schema_file: json-schema/apache-samza-job-schema.json
slug: apache-samza-job
tags:
- Big Data
- Hadoop
- Kafka
- Stream Processing
- Streaming
- Apache
- Open Source
title: Job
---
