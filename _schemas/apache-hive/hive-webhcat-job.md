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
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hive/json-schema/hive-webhcat-job-schema.json\",\n  \"title\": \"Job\",\n  \"type\": \"object\",\n  \"description\": \"WebHCat Hive job submission\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID\",\n      \"example\": \"job_1718153645993_0001\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Job status\",\n      \"example\": \"RUNNING\"\n    },\n    \"percentComplete\": {\n      \"type\": \"string\",\n      \"description\": \"Job completion percentage\",\n      \"example\": \"50% complete\"\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"HiveQL query string\",\n      \"example\": \"SELECT COUNT(*) FROM sales\"\n    },\n    \"database\": {\n      \"type\": \"string\",\n      \"description\": \"Target database\",\n      \"example\": \"mydb\"\n\
  \    },\n    \"statusdir\": {\n      \"type\": \"string\",\n      \"description\": \"HDFS directory for output and status\",\n      \"example\": \"/tmp/hive-output\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hive/refs/heads/main/json-schema/hive-webhcat-job-schema.json
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
