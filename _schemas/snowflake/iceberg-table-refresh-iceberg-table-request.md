---
description: Request model for refreshing iceberg table
layout: schema
name: RefreshIcebergTableRequest
properties_list:
- description: Specifies a metadata file path for a table created from Iceberg files in object storage.
  name: metadata_file_relative_path
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/iceberg-table-refresh-iceberg-table-request-schema.json
slug: iceberg-table-refresh-iceberg-table-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RefreshIcebergTableRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request model for refreshing iceberg table\",\n  \"properties\": {\n    \"metadata_file_relative_path\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies a metadata file path for a table created from Iceberg files in object storage.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/iceberg-table-refresh-iceberg-table-request-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: RefreshIcebergTableRequest
---
