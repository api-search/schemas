---
description: Schema definition for an Apache Doris table, describing columns, keys, and partitioning.
layout: schema
name: TableSchema
properties_list:
- description: Name of the table.
  name: tableName
  type: string
- description: Database containing the table.
  name: databaseName
  type: string
- description: Data model of the table.
  name: tableType
  type: string
- description: Key model for the table.
  name: keyType
  type: string
- description: List of column definitions.
  name: columns
  type: array
- description: Table comment.
  name: comment
  type: string
- description: Number of data replicas.
  name: replicationNum
  type: integer
provider_name: Apache Doris
provider_slug: apache-doris
schema_file: json-schema/apache-doris-table-schema-schema.json
slug: apache-doris-table-schema
source_filename: apache-doris-table-schema-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-doris/refs/heads/main/json-schema/apache-doris-table-schema-schema.json\",\n  \"title\": \"TableSchema\",\n  \"description\": \"Schema definition for an Apache Doris table, describing columns, keys, and partitioning.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tableName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the table.\",\n      \"example\": \"sales_events\"\n    },\n    \"databaseName\": {\n      \"type\": \"string\",\n      \"description\": \"Database containing the table.\",\n      \"example\": \"analytics\"\n    },\n    \"tableType\": {\n      \"type\": \"string\",\n      \"description\": \"Data model of the table.\",\n      \"enum\": [\n        \"OLAP\",\n        \"EXTERNAL\",\n        \"MYSQL\",\n        \"BROKER\",\n        \"HIVE\"\n      ],\n      \"example\": \"OLAP\"\n    },\n    \"keyType\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Key model for the table.\",\n      \"enum\": [\n        \"DUP_KEYS\",\n        \"AGG_KEYS\",\n        \"UNIQUE_KEYS\"\n      ],\n      \"example\": \"DUP_KEYS\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"description\": \"List of column definitions.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Column name.\",\n            \"example\": \"event_time\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Doris data type.\",\n            \"example\": \"DATETIME\"\n          },\n          \"isKey\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether this column is part of the key.\",\n            \"example\": false\n          },\n          \"nullable\": {\n            \"type\": \"boolean\",\n            \"description\"\
  : \"Whether this column allows NULL values.\",\n            \"example\": true\n          },\n          \"comment\": {\n            \"type\": \"string\",\n            \"description\": \"Column comment.\",\n            \"example\": \"Timestamp of the event\"\n          }\n        }\n      }\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Table comment.\",\n      \"example\": \"Sales event records table\"\n    },\n    \"replicationNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of data replicas.\",\n      \"default\": 3,\n      \"example\": 3\n    }\n  },\n  \"required\": [\n    \"tableName\",\n    \"databaseName\",\n    \"keyType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-doris/refs/heads/main/json-schema/apache-doris-table-schema-schema.json
tags:
- Analytics
- Apache
- Database
- Lakehouse
- MPP
- OLAP
- Open Source
- Real-Time
- SQL
title: TableSchema
---
