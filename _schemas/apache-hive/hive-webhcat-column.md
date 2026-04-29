---
description: Hive table column definition
layout: schema
name: Column
properties_list:
- description: Column name
  name: name
  type: string
- description: Column data type
  name: type
  type: string
- description: Column description
  name: comment
  type: string
provider_name: Apache Hive
provider_slug: apache-hive
schema_file: json-schema/hive-webhcat-column-schema.json
slug: hive-webhcat-column
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hive/json-schema/hive-webhcat-column-schema.json\",\n  \"title\": \"Column\",\n  \"type\": \"object\",\n  \"description\": \"Hive table column definition\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Column name\",\n      \"example\": \"order_id\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Column data type\",\n      \"example\": \"BIGINT\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Column description\",\n      \"example\": \"Unique order identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hive/refs/heads/main/json-schema/hive-webhcat-column-schema.json
tags:
- Apache
- Big Data
- Data Warehouse
- ETL
- Hadoop
- Open Source
- SQL
title: Column
---
