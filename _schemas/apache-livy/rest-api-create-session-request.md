---
description: Parameters for creating an interactive session
layout: schema
name: CreateSessionRequest
properties_list:
- description: Session programming language
  name: kind
  type: string
- description: User to impersonate when running the session
  name: proxyUser
  type: string
- description: JARs to include on the classpath
  name: jars
  type: array
- description: Python files to include
  name: pyFiles
  type: array
- description: Files to include
  name: files
  type: array
- description: Driver memory amount
  name: driverMemory
  type: string
- description: Number of driver cores
  name: driverCores
  type: integer
- description: Executor memory amount
  name: executorMemory
  type: string
- description: Number of executor cores
  name: executorCores
  type: integer
- description: Number of executors
  name: numExecutors
  type: integer
- description: Spark configuration key-value pairs
  name: conf
  type: object
provider_name: Apache Livy
provider_slug: apache-livy
schema_file: json-schema/rest-api-create-session-request-schema.json
slug: rest-api-create-session-request
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: CreateSessionRequest
---
