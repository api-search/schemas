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
source_filename: rest-api-create-session-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-create-session-request-schema.json\",\n  \"title\": \"CreateSessionRequest\",\n  \"description\": \"Parameters for creating an interactive session\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Session programming language\",\n      \"enum\": [\n        \"spark\",\n        \"pyspark\",\n        \"sparkr\",\n        \"sql\"\n      ],\n      \"example\": \"pyspark\"\n    },\n    \"proxyUser\": {\n      \"type\": \"string\",\n      \"description\": \"User to impersonate when running the session\",\n      \"example\": \"alice\"\n    },\n    \"jars\": {\n      \"type\": \"array\",\n      \"description\": \"JARs to include on the classpath\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"pyFiles\": {\n\
  \      \"type\": \"array\",\n      \"description\": \"Python files to include\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"description\": \"Files to include\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"driverMemory\": {\n      \"type\": \"string\",\n      \"description\": \"Driver memory amount\",\n      \"example\": \"512m\"\n    },\n    \"driverCores\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of driver cores\",\n      \"example\": 1\n    },\n    \"executorMemory\": {\n      \"type\": \"string\",\n      \"description\": \"Executor memory amount\",\n      \"example\": \"1g\"\n    },\n    \"executorCores\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of executor cores\",\n      \"example\": 1\n    },\n    \"numExecutors\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of executors\",\n      \"example\": 2\n    },\n\
  \    \"conf\": {\n      \"type\": \"object\",\n      \"description\": \"Spark configuration key-value pairs\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-create-session-request-schema.json
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: CreateSessionRequest
---
