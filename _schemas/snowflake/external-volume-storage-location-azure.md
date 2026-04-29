---
description: ''
layout: schema
name: StorageLocationAzure
properties_list:
- description: Specifies the ID for your Office 365 tenant that the allowed and blocked storage accounts belong to.
  name: azure_tenant_id
  type: string
- description: Specifies the base URL for your cloud storage location.
  name: storage_base_url
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/external-volume-storage-location-azure-schema.json
slug: external-volume-storage-location-azure
source_filename: external-volume-storage-location-azure-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StorageLocationAzure\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"azure_tenant_id\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the ID for your Office 365 tenant that the allowed and blocked storage accounts belong to.\"\n    },\n    \"storage_base_url\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the base URL for your cloud storage location.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/external-volume-storage-location-azure-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: StorageLocationAzure
---
