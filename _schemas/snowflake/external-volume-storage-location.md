---
description: ''
layout: schema
name: StorageLocation
properties_list:
- description: ''
  name: name
  type: string
- description: Specifies the cloud storage provider that stores your data files.
  name: storage_provider
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/external-volume-storage-location-schema.json
slug: external-volume-storage-location
source_filename: external-volume-storage-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StorageLocation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"\"\n    },\n    \"storage_provider\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the cloud storage provider that stores your data files.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/external-volume-storage-location-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: StorageLocation
---
