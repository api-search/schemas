---
description: A document stored in a SODA collection in Oracle Database 19c.
layout: schema
name: SODA Document
properties_list:
- description: Document key
  name: id
  type: string
- description: ''
  name: etag
  type: string
- description: ''
  name: lastModified
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: mediaType
  type: string
- description: ''
  name: version
  type: string
- description: JSON content of the document
  name: value
  type: object
provider_name: Oracle Database 19c
provider_slug: oracle-database-19c
schema_file: json-schema/oracle-database-19c-soda-document.json
slug: oracle-database-19c-soda-document
source_filename: oracle-database-19c-soda-document.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-database-19c/main/json-schema/oracle-database-19c-soda-document.json\",\n  \"title\": \"SODA Document\",\n  \"description\": \"A document stored in a SODA collection in Oracle Database 19c.\",\n  \"type\": \"object\",\n  \"required\": [\"id\"],\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Document key\" },\n    \"etag\": { \"type\": \"string\" },\n    \"lastModified\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"created\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"mediaType\": { \"type\": \"string\", \"default\": \"application/json\" },\n    \"version\": { \"type\": \"string\" },\n    \"value\": {\n      \"description\": \"JSON content of the document\",\n      \"oneOf\": [\n        { \"type\": \"object\", \"additionalProperties\": true },\n        { \"type\": \"array\" }\n\
  \      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-database-19c/refs/heads/main/json-schema/oracle-database-19c-soda-document.json
tags:
- Database
- Enterprise
- Json
- Machine-Learning
- Nosql
- Oracle
- Rest
- Sql
title: SODA Document
---
