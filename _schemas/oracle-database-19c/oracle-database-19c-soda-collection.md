---
description: A SODA (Simple Oracle Document Access) collection in Oracle Database 19c.
layout: schema
name: SODA Collection
properties_list:
- description: Collection name
  name: name
  type: string
- description: Owning database schema
  name: schemaName
  type: string
- description: ''
  name: keyColumn
  type: object
- description: ''
  name: contentColumn
  type: object
- description: ''
  name: versionColumn
  type: object
- description: ''
  name: lastModifiedColumn
  type: object
- description: ''
  name: creationTimeColumn
  type: object
- description: ''
  name: mediaTypeColumn
  type: object
- description: ''
  name: readOnly
  type: boolean
provider_name: Oracle Database 19c
provider_slug: oracle-database-19c
schema_file: json-schema/oracle-database-19c-soda-collection.json
slug: oracle-database-19c-soda-collection
source_filename: oracle-database-19c-soda-collection.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-database-19c/main/json-schema/oracle-database-19c-soda-collection.json\",\n  \"title\": \"SODA Collection\",\n  \"description\": \"A SODA (Simple Oracle Document Access) collection in Oracle Database 19c.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Collection name\"\n    },\n    \"schemaName\": {\n      \"type\": \"string\",\n      \"description\": \"Owning database schema\"\n    },\n    \"keyColumn\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"sqlType\": { \"type\": \"string\", \"enum\": [\"VARCHAR2\", \"NUMBER\", \"RAW\"] },\n        \"maxLength\": { \"type\": \"integer\" },\n        \"assignmentMethod\": { \"type\": \"string\", \"enum\": [\"UUID\", \"SEQUENCE\", \"\
  GUID\", \"CLIENT\"] }\n      }\n    },\n    \"contentColumn\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"sqlType\": { \"type\": \"string\", \"enum\": [\"BLOB\", \"CLOB\", \"VARCHAR2\", \"JSON\"] },\n        \"validation\": { \"type\": \"string\", \"enum\": [\"STANDARD\", \"STRICT\"] },\n        \"compress\": { \"type\": \"string\" },\n        \"cache\": { \"type\": \"boolean\" },\n        \"encrypt\": { \"type\": \"string\" }\n      }\n    },\n    \"versionColumn\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"method\": { \"type\": \"string\", \"enum\": [\"NONE\", \"UUID\", \"TIMESTAMP\", \"SHA256\", \"MD5\", \"SEQUENTIAL\"] }\n      }\n    },\n    \"lastModifiedColumn\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"index\": { \"type\": \"string\" }\n      }\n    },\n    \"creationTimeColumn\"\
  : {\n      \"type\": \"object\",\n      \"properties\": { \"name\": { \"type\": \"string\" } }\n    },\n    \"mediaTypeColumn\": {\n      \"type\": \"object\",\n      \"properties\": { \"name\": { \"type\": \"string\" } }\n    },\n    \"readOnly\": { \"type\": \"boolean\", \"default\": false }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-database-19c/refs/heads/main/json-schema/oracle-database-19c-soda-collection.json
tags:
- Database
- Enterprise
- Json
- Machine-Learning
- Nosql
- Oracle
- Rest
- Sql
title: SODA Collection
---
