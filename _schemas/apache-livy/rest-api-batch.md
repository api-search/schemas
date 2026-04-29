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
source_filename: rest-api-batch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-batch-schema.json\",\n  \"title\": \"Batch\",\n  \"description\": \"A batch Spark job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Batch identifier\",\n      \"example\": 0\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"Spark application ID\",\n      \"example\": \"application_1234567890_0001\"\n    },\n    \"appInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Spark application information\"\n    },\n    \"log\": {\n      \"type\": \"array\",\n      \"description\": \"Recent log lines\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Batch state\",\n      \"enum\": [\n        \"not_started\"\
  ,\n        \"starting\",\n        \"running\",\n        \"dead\",\n        \"shutting_down\",\n        \"success\"\n      ],\n      \"example\": \"success\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-batch-schema.json
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: Batch
---
