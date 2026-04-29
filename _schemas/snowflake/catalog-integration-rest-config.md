---
description: ''
layout: schema
name: RestConfig
properties_list:
- description: Customer's Polaris account locator URL
  name: catalog_uri
  type: string
- description: Name of the catalog to use in Polaris
  name: warehouse
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/catalog-integration-rest-config-schema.json
slug: catalog-integration-rest-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RestConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"catalog_uri\": {\n      \"type\": \"string\",\n      \"description\": \"Customer's Polaris account locator URL\"\n    },\n    \"warehouse\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the catalog to use in Polaris\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/catalog-integration-rest-config-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: RestConfig
---
