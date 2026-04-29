---
description: Information about a partition of the result set.
layout: schema
name: PartitionInfo
properties_list:
- description: Number of rows in the partition.
  name: rowCount
  type: integer
- description: The partition size before decompression. This may not be present in every partition.
  name: compressedSize
  type: integer
- description: The partition size after decompression.
  name: uncompressedSize
  type: integer
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/snowflake-sql-rest-partition-info-schema.json
slug: snowflake-sql-rest-partition-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PartitionInfo\",\n  \"type\": \"object\",\n  \"description\": \"Information about a partition of the result set.\",\n  \"properties\": {\n    \"rowCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows in the partition.\"\n    },\n    \"compressedSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The partition size before decompression. This may not be present in every partition.\"\n    },\n    \"uncompressedSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The partition size after decompression.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/snowflake-sql-rest-partition-info-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: PartitionInfo
---
