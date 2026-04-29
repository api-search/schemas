---
description: Create iceberg table as select
layout: schema
name: IcebergTableAsSelect
properties_list:
- description: Specifies the name for the table, must be unique for the schema in which the table is created
  name: name
  type: string
- description: ''
  name: columns
  type: array
- description: Specifies the name of the external volume to use for the table
  name: external_volume
  type: string
- description: Specifies one or more columns or column expressions in the table as the clustering key
  name: cluster_by
  type: array
- description: Specifies the path to a directory where Snowflake can write data and metadata files for the table
  name: base_location
  type: string
- description: Specifies a comment for the table
  name: comment
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/iceberg-table-iceberg-table-as-select-schema.json
slug: iceberg-table-iceberg-table-as-select
source_filename: iceberg-table-iceberg-table-as-select-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IcebergTableAsSelect\",\n  \"type\": \"object\",\n  \"description\": \"Create iceberg table as select\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the name for the table, must be unique for the schema in which the table is created\"\n    },\n    \"columns\": {\n      \"type\": \"array\"\n    },\n    \"external_volume\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the name of the external volume to use for the table\"\n    },\n    \"cluster_by\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies one or more columns or column expressions in the table as the clustering key\"\n    },\n    \"base_location\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the path to a directory where Snowflake can write data and metadata files for the table\"\n    },\n    \"comment\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Specifies a comment for the table\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/iceberg-table-iceberg-table-as-select-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: IcebergTableAsSelect
---
