---
description: ''
layout: schema
name: ColumnMetadata
properties_list:
- description: The name of the column
  name: name
  type: string
- description: The label of the column (display name)
  name: label
  type: string
- description: The database-specific data type name of the column
  name: typeName
  type: string
- description: The default value for the column
  name: columnDefault
  type: string
- description: Whether the column is case-sensitive
  name: isCaseSensitive
  type: boolean
- description: Whether the column contains currency data
  name: isCurrency
  type: boolean
- description: Whether the column values are signed numbers
  name: isSigned
  type: boolean
- description: Indicates the nullability of the column. 0 = not nullable, 1 = nullable, 2 = unknown.
  name: nullable
  type: integer
- description: The precision of the column for numeric types
  name: precision
  type: integer
- description: The scale of the column for numeric types
  name: scale
  type: integer
- description: The length of the column for character types
  name: length
  type: integer
- description: The schema name that contains the table
  name: schemaName
  type: string
- description: The name of the table that contains the column
  name: tableName
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-column-metadata-schema.json
slug: amazon-redshift-data-column-metadata
source_filename: amazon-redshift-data-column-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ColumnMetadata\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the column\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The label of the column (display name)\"\n    },\n    \"typeName\": {\n      \"type\": \"string\",\n      \"description\": \"The database-specific data type name of the column\"\n    },\n    \"columnDefault\": {\n      \"type\": \"string\",\n      \"description\": \"The default value for the column\"\n    },\n    \"isCaseSensitive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the column is case-sensitive\"\n    },\n    \"isCurrency\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the column contains currency data\"\n    },\n    \"isSigned\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the column\
  \ values are signed numbers\"\n    },\n    \"nullable\": {\n      \"type\": \"integer\",\n      \"description\": \"Indicates the nullability of the column. 0 = not nullable, 1 = nullable, 2 = unknown.\"\n    },\n    \"precision\": {\n      \"type\": \"integer\",\n      \"description\": \"The precision of the column for numeric types\"\n    },\n    \"scale\": {\n      \"type\": \"integer\",\n      \"description\": \"The scale of the column for numeric types\"\n    },\n    \"length\": {\n      \"type\": \"integer\",\n      \"description\": \"The length of the column for character types\"\n    },\n    \"schemaName\": {\n      \"type\": \"string\",\n      \"description\": \"The schema name that contains the table\"\n    },\n    \"tableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table that contains the column\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-column-metadata-schema.json
tags:
- Analytics
- Big Data
- Cloud
- Data Lake
- Data Warehouse
- ETL
- Machine Learning
- Serverless
- SQL
title: ColumnMetadata
---
