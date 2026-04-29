---
description: Hive database (schema) in the metastore
layout: schema
name: Database
properties_list:
- description: Database name
  name: name
  type: string
- description: Database description
  name: comment
  type: string
- description: HDFS location URI
  name: location
  type: string
- description: Owner of the database
  name: ownerName
  type: string
- description: Owner type (USER or ROLE)
  name: ownerType
  type: string
provider_name: Apache Hive
provider_slug: apache-hive
schema_file: json-schema/hive-webhcat-database-schema.json
slug: hive-webhcat-database
source_filename: hive-webhcat-database-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hive/json-schema/hive-webhcat-database-schema.json\",\n  \"title\": \"Database\",\n  \"type\": \"object\",\n  \"description\": \"Hive database (schema) in the metastore\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Database name\",\n      \"example\": \"mydb\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Database description\",\n      \"example\": \"My analytics database\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"HDFS location URI\",\n      \"example\": \"hdfs://namenode/user/hive/warehouse/mydb.db\"\n    },\n    \"ownerName\": {\n      \"type\": \"string\",\n      \"description\": \"Owner of the database\",\n      \"example\": \"hive\"\n    },\n    \"ownerType\": {\n      \"type\": \"string\",\n      \"description\": \"Owner type\
  \ (USER or ROLE)\",\n      \"example\": \"USER\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hive/refs/heads/main/json-schema/hive-webhcat-database-schema.json
tags:
- Apache
- Big Data
- Data Warehouse
- ETL
- Hadoop
- Open Source
- SQL
title: Database
---
