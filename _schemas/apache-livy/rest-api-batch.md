---
description: A batch Spark job
layout: schema
name: Batch
properties_list:
- description: Batch identifier
  name: id
  type: integer
- description: Spark application ID
  name: appId
  type: string
- description: Spark application information
  name: appInfo
  type: object
- description: Recent log lines
  name: log
  type: array
- description: Batch state
  name: state
  type: string
provider_name: Apache Livy
provider_slug: apache-livy
schema_file: json-schema/rest-api-batch-schema.json
slug: rest-api-batch
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: Batch
---
