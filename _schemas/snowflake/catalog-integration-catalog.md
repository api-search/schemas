---
description: ''
layout: schema
name: Catalog
properties_list:
- description: Type of external catalog
  name: catalog_source
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/catalog-integration-catalog-schema.json
slug: catalog-integration-catalog
source_filename: catalog-integration-catalog-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Catalog\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"catalog_source\": {\n      \"type\": \"string\",\n      \"description\": \"Type of external catalog\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/catalog-integration-catalog-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Catalog
---
