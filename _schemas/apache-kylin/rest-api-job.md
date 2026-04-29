---
description: A Kylin build job
layout: schema
name: Job
properties_list:
- description: ''
  name: uuid
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: relatedCube
  type: string
- description: ''
  name: relatedSegment
  type: string
- description: ''
  name: status
  type: string
- description: Submit time as Unix timestamp
  name: submitTime
  type: integer
- description: Job duration in seconds
  name: duration
  type: integer
- description: MapReduce waiting time
  name: mrWaiting
  type: integer
provider_name: Apache Kylin
provider_slug: apache-kylin
schema_file: json-schema/rest-api-job-schema.json
slug: rest-api-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-job-schema.json\",\n  \"title\": \"Job\",\n  \"description\": \"A Kylin build job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"example\": \"job-1234\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"BUILD CUBE - kylin_sales_cube\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"BUILD\"\n    },\n    \"relatedCube\": {\n      \"type\": \"string\",\n      \"example\": \"kylin_sales_cube\"\n    },\n    \"relatedSegment\": {\n      \"type\": \"string\",\n      \"example\": \"segment-1234\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"READY\",\n        \"RUNNING\",\n        \"ERROR\",\n        \"STOPPED\",\n        \"FINISHED\",\n        \"DISCARDED\"\
  \n      ],\n      \"example\": \"FINISHED\"\n    },\n    \"submitTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Submit time as Unix timestamp\",\n      \"example\": 1718153645993\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Job duration in seconds\",\n      \"example\": 120\n    },\n    \"mrWaiting\": {\n      \"type\": \"integer\",\n      \"description\": \"MapReduce waiting time\",\n      \"example\": 10\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-job-schema.json
tags:
- Analytics
- Big Data
- Cube
- OLAP
- Open Source
- SQL
title: Job
---
