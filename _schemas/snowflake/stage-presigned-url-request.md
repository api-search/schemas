---
description: Request object to get presigned url of a file
layout: schema
name: PresignedUrlRequest
properties_list:
- description: Expiration time of the generated presigned url in seconds.
  name: expiration_time
  type: integer
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/stage-presigned-url-request-schema.json
slug: stage-presigned-url-request
source_filename: stage-presigned-url-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PresignedUrlRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request object to get presigned url of a file\",\n  \"properties\": {\n    \"expiration_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Expiration time of the generated presigned url in seconds.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/stage-presigned-url-request-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: PresignedUrlRequest
---
