---
description: Result of a WebHCat DDL or DML operation
layout: schema
name: QueryResult
properties_list:
- description: HTTP status code
  name: status
  type: integer
- description: Result schema as JSON string
  name: schema
  type: string
- description: Result rows
  name: rows
  type: array
- description: Active database
  name: database
  type: string
provider_name: Apache Hive
provider_slug: apache-hive
schema_file: json-schema/hive-webhcat-queryresult-schema.json
slug: hive-webhcat-queryresult
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hive/json-schema/hive-webhcat-queryresult-schema.json\",\n  \"title\": \"QueryResult\",\n  \"type\": \"object\",\n  \"description\": \"Result of a WebHCat DDL or DML operation\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code\",\n      \"example\": 200\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"Result schema as JSON string\",\n      \"example\": \"\"\n    },\n    \"rows\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Result rows\"\n    },\n    \"database\": {\n      \"type\": \"string\",\n      \"description\": \"Active database\",\n      \"example\": \"mydb\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hive/refs/heads/main/json-schema/hive-webhcat-queryresult-schema.json
tags:
- Apache
- Big Data
- Data Warehouse
- ETL
- Hadoop
- Open Source
- SQL
title: QueryResult
---
