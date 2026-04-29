---
description: Materials for uploading and downloading stage files
layout: schema
name: FileTransferMaterial
properties_list:
- description: Presigned url for file transfer, only works for Server Side Encrypted Stages.
  name: presigned_url
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/stage-file-transfer-material-schema.json
slug: stage-file-transfer-material
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FileTransferMaterial\",\n  \"type\": \"object\",\n  \"description\": \"Materials for uploading and downloading stage files\",\n  \"properties\": {\n    \"presigned_url\": {\n      \"type\": \"string\",\n      \"description\": \"Presigned url for file transfer, only works for Server Side Encrypted Stages.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/stage-file-transfer-material-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: FileTransferMaterial
---
