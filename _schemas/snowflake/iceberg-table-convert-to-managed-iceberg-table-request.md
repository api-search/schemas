---
description: Request model for convert to managed iceberg table
layout: schema
name: ConvertToManagedIcebergTableRequest
properties_list:
- description: The path to a directory where Snowflake can write data and metadata files for the table.
  name: base_location
  type: string
- description: Specifies the storage serialization policy for the table.
  name: storage_serialization_policy
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/iceberg-table-convert-to-managed-iceberg-table-request-schema.json
slug: iceberg-table-convert-to-managed-iceberg-table-request
source_filename: iceberg-table-convert-to-managed-iceberg-table-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConvertToManagedIcebergTableRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request model for convert to managed iceberg table\",\n  \"properties\": {\n    \"base_location\": {\n      \"type\": \"string\",\n      \"description\": \"The path to a directory where Snowflake can write data and metadata files for the table.\"\n    },\n    \"storage_serialization_policy\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the storage serialization policy for the table.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/iceberg-table-convert-to-managed-iceberg-table-request-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ConvertToManagedIcebergTableRequest
---
