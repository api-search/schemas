---
description: Catalog integration
layout: schema
name: CatalogIntegration
properties_list:
- description: Name of the catalog integration.
  name: name
  type: string
- description: Table format of the catalog.
  name: table_format
  type: string
- description: whether this catalog integration is available to use for Iceberg tables.
  name: enabled
  type: boolean
- description: Comment.
  name: comment
  type: string
- description: Type of the integration. Always CATALOG.
  name: type
  type: string
- description: Category of the integration. Always CATALOG.
  name: category
  type: string
- description: Date and time when the catalog integration was created.
  name: created_on
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/catalog-integration-catalog-integration-schema.json
slug: catalog-integration-catalog-integration
source_filename: catalog-integration-catalog-integration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CatalogIntegration\",\n  \"type\": \"object\",\n  \"description\": \"Catalog integration\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the catalog integration.\"\n    },\n    \"table_format\": {\n      \"type\": \"string\",\n      \"description\": \"Table format of the catalog.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"whether this catalog integration is available to use for Iceberg tables. \"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Comment.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the integration. Always CATALOG.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the integration. Always CATALOG.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Date and time when the catalog integration was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/catalog-integration-catalog-integration-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: CatalogIntegration
---
