---
description: Create iceberg table from Delta
layout: schema
name: IcebergTableFromDelta
properties_list:
- description: Specifies the name for the table, must be unique for the schema in which the table is created
  name: name
  type: string
- description: Specifies the name of the external volume to use for the table
  name: external_volume
  type: string
- description: Specifies whether to replace invalid characters in the column names
  name: replace_invalid_characters
  type: boolean
- description: Specifies a relative path from the table’s EXTERNAL_VOLUME location to a directory where Snowflake can access your Delta table files.
  name: base_location
  type: string
- description: Specifies the name of the catalog integration to use for the table
  name: catalog
  type: string
- description: Specifies a comment for the table
  name: comment
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/iceberg-table-iceberg-table-from-delta-schema.json
slug: iceberg-table-iceberg-table-from-delta
source_filename: iceberg-table-iceberg-table-from-delta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IcebergTableFromDelta\",\n  \"type\": \"object\",\n  \"description\": \"Create iceberg table from Delta\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the name for the table, must be unique for the schema in which the table is created\"\n    },\n    \"external_volume\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the name of the external volume to use for the table\"\n    },\n    \"replace_invalid_characters\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether to replace invalid characters in the column names\"\n    },\n    \"base_location\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies a relative path from the table\\u2019s EXTERNAL_VOLUME location to a directory where Snowflake can access your Delta table files.\"\n    },\n    \"catalog\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Specifies the name of the catalog integration to use for the table\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies a comment for the table\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/iceberg-table-iceberg-table-from-delta-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: IcebergTableFromDelta
---
