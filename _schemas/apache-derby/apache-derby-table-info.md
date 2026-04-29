---
description: Metadata about a table in an Apache Derby database, as returned by JDBC DatabaseMetaData.getTables().
layout: schema
name: TableInfo
properties_list:
- description: Name of the table.
  name: tableName
  type: string
- description: Schema (owner) of the table.
  name: tableSchema
  type: string
- description: Catalog of the table (always null in Derby).
  name: tableCatalog
  type: string
- description: Type of table object.
  name: tableType
  type: string
- description: Table comment if defined.
  name: remarks
  type: string
provider_name: Apache Derby
provider_slug: apache-derby
schema_file: json-schema/apache-derby-table-info-schema.json
slug: apache-derby-table-info
source_filename: apache-derby-table-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-derby/refs/heads/main/json-schema/apache-derby-table-info-schema.json\",\n  \"title\": \"TableInfo\",\n  \"description\": \"Metadata about a table in an Apache Derby database, as returned by JDBC DatabaseMetaData.getTables().\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tableName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the table.\",\n      \"example\": \"EMPLOYEES\"\n    },\n    \"tableSchema\": {\n      \"type\": \"string\",\n      \"description\": \"Schema (owner) of the table.\",\n      \"example\": \"APP\"\n    },\n    \"tableCatalog\": {\n      \"type\": \"string\",\n      \"description\": \"Catalog of the table (always null in Derby).\",\n      \"example\": null\n    },\n    \"tableType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of table object.\",\n      \"enum\": [\n   \
  \     \"TABLE\",\n        \"VIEW\",\n        \"SYSTEM TABLE\",\n        \"SYNONYM\"\n      ],\n      \"example\": \"TABLE\"\n    },\n    \"remarks\": {\n      \"type\": \"string\",\n      \"description\": \"Table comment if defined.\",\n      \"example\": \"Employee records table\"\n    }\n  },\n  \"required\": [\n    \"tableName\",\n    \"tableType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-derby/refs/heads/main/json-schema/apache-derby-table-info-schema.json
tags:
- Apache
- Database
- Embedded
- Java
- JDBC
- Open Source
- Relational
- SQL
title: TableInfo
---
