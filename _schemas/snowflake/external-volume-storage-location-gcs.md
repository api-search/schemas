---
description: ''
layout: schema
name: StorageLocationGcs
properties_list:
- description: Specifies the base URL for your cloud storage location.
  name: storage_base_url
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/external-volume-storage-location-gcs-schema.json
slug: external-volume-storage-location-gcs
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StorageLocationGcs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"storage_base_url\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the base URL for your cloud storage location.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/external-volume-storage-location-gcs-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: StorageLocationGcs
---
