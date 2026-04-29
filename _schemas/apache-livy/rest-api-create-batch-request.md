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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-create-batch-request-schema.json\",\n  \"title\": \"CreateBatchRequest\",\n  \"description\": \"Parameters for creating a batch Spark job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"file\": {\n      \"type\": \"string\",\n      \"description\": \"File to execute\",\n      \"example\": \"s3://my-bucket/jobs/my-spark-job.py\"\n    },\n    \"proxyUser\": {\n      \"type\": \"string\",\n      \"description\": \"User to impersonate\",\n      \"example\": \"alice\"\n    },\n    \"className\": {\n      \"type\": \"string\",\n      \"description\": \"Application Java/Spark main class\",\n      \"example\": \"com.example.MySparkJob\"\n    },\n    \"args\": {\n      \"type\": \"array\",\n      \"description\": \"Command line arguments\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n\
  \    },\n    \"jars\": {\n      \"type\": \"array\",\n      \"description\": \"JARs to include\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"pyFiles\": {\n      \"type\": \"array\",\n      \"description\": \"Python files\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"driverMemory\": {\n      \"type\": \"string\",\n      \"description\": \"Driver memory\",\n      \"example\": \"512m\"\n    },\n    \"executorMemory\": {\n      \"type\": \"string\",\n      \"description\": \"Executor memory\",\n      \"example\": \"1g\"\n    },\n    \"numExecutors\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of executors\",\n      \"example\": 4\n    },\n    \"conf\": {\n      \"type\": \"object\",\n      \"description\": \"Spark configuration\"\n    }\n  },\n  \"required\": [\n    \"file\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-create-batch-request-schema.json
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: CreateBatchRequest
---
