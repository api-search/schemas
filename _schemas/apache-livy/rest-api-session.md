---
description: An interactive Spark session
layout: schema
name: Session
properties_list:
- description: Session identifier
  name: id
  type: integer
- description: Spark application ID
  name: appId
  type: string
- description: Session owner
  name: owner
  type: string
- description: Proxy user for the session
  name: proxyUser
  type: string
- description: Session type
  name: kind
  type: string
- description: Recent log lines
  name: log
  type: array
- description: Session state
  name: state
  type: string
- description: Spark application information
  name: appInfo
  type: object
provider_name: Apache Livy
provider_slug: apache-livy
schema_file: json-schema/rest-api-session-schema.json
slug: rest-api-session
source_filename: rest-api-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-session-schema.json\",\n  \"title\": \"Session\",\n  \"description\": \"An interactive Spark session\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Session identifier\",\n      \"example\": 0\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"Spark application ID\",\n      \"example\": \"application_1234567890_0001\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Session owner\",\n      \"example\": \"hdfs\"\n    },\n    \"proxyUser\": {\n      \"type\": \"string\",\n      \"description\": \"Proxy user for the session\",\n      \"example\": \"alice\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Session type\",\n      \"enum\": [\n\
  \        \"spark\",\n        \"pyspark\",\n        \"sparkr\",\n        \"sql\"\n      ],\n      \"example\": \"pyspark\"\n    },\n    \"log\": {\n      \"type\": \"array\",\n      \"description\": \"Recent log lines\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Session state\",\n      \"enum\": [\n        \"not_started\",\n        \"starting\",\n        \"idle\",\n        \"busy\",\n        \"shutting_down\",\n        \"error\",\n        \"dead\",\n        \"killed\",\n        \"success\"\n      ],\n      \"example\": \"idle\"\n    },\n    \"appInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Spark application information\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-session-schema.json
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: Session
---
