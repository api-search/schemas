---
description: WebHCat Hive job submission
layout: schema
name: Job
properties_list:
- description: Job ID
  name: id
  type: string
- description: Job status
  name: status
  type: string
- description: Job completion percentage
  name: percentComplete
  type: string
- description: HiveQL query string
  name: query
  type: string
- description: Target database
  name: database
  type: string
- description: HDFS directory for output and status
  name: statusdir
  type: string
provider_name: Apache Hive
provider_slug: apache-hive
schema_file: json-schema/hive-webhcat-job-schema.json
slug: hive-webhcat-job
tags:
- Apache
- Big Data
- Data Warehouse
- ETL
- Hadoop
- Open Source
- SQL
title: Job
---
