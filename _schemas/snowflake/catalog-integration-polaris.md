---
description: ''
layout: schema
name: Polaris
properties_list:
- description: Default Polaris namespace used by all Iceberg tables associated with this catalog integration
  name: catalog_namespace
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/catalog-integration-polaris-schema.json
slug: catalog-integration-polaris
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Polaris\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"catalog_namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Default Polaris namespace used by all Iceberg tables associated with this catalog integration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/catalog-integration-polaris-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Polaris
---
