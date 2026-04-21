---
description: Parameters for creating a batch Spark job
layout: schema
name: CreateBatchRequest
properties_list:
- description: File to execute
  name: file
  type: string
- description: User to impersonate
  name: proxyUser
  type: string
- description: Application Java/Spark main class
  name: className
  type: string
- description: Command line arguments
  name: args
  type: array
- description: JARs to include
  name: jars
  type: array
- description: Python files
  name: pyFiles
  type: array
- description: Driver memory
  name: driverMemory
  type: string
- description: Executor memory
  name: executorMemory
  type: string
- description: Number of executors
  name: numExecutors
  type: integer
- description: Spark configuration
  name: conf
  type: object
provider_name: Apache Livy
provider_slug: apache-livy
schema_file: json-schema/rest-api-create-batch-request-schema.json
slug: rest-api-create-batch-request
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: CreateBatchRequest
---
