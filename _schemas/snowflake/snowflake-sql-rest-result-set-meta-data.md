---
description: Metadata about the result set including column definitions.
layout: schema
name: ResultSetMetaData
properties_list:
- description: For v2 endpoints the only possible value for this field is jsonv2.
  name: format
  type: string
- description: The total number of rows of results.
  name: numRows
  type: integer
- description: Array of column descriptors for the result set.
  name: rowType
  type: array
- description: Information about result set partitions for large results.
  name: partitionInfo
  type: array
- description: If false, null values are replaced with the string 'null' in the result set.
  name: nullable
  type: boolean
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/snowflake-sql-rest-result-set-meta-data-schema.json
slug: snowflake-sql-rest-result-set-meta-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResultSetMetaData\",\n  \"type\": \"object\",\n  \"description\": \"Metadata about the result set including column definitions.\",\n  \"properties\": {\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"For v2 endpoints the only possible value for this field is jsonv2.\"\n    },\n    \"numRows\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of rows of results.\"\n    },\n    \"rowType\": {\n      \"type\": \"array\",\n      \"description\": \"Array of column descriptors for the result set.\"\n    },\n    \"partitionInfo\": {\n      \"type\": \"array\",\n      \"description\": \"Information about result set partitions for large results.\"\n    },\n    \"nullable\": {\n      \"type\": \"boolean\",\n      \"description\": \"If false, null values are replaced with the string 'null' in the result set.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/snowflake-sql-rest-result-set-meta-data-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ResultSetMetaData
---
