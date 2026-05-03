---
description: Represents a JSON document stored in an Oracle SODA collection, including metadata such as key, version, and timestamps managed by the database.
layout: schema
name: Oracle SODA Document
properties_list:
- description: Unique document key assigned by the server or client
  name: id
  type: string
- description: Entity tag representing the document version for optimistic concurrency control
  name: etag
  type: string
- description: Timestamp of the last modification to the document
  name: lastModified
  type: string
- description: Timestamp when the document was created
  name: created
  type: string
- description: The JSON document content
  name: value
  type: object
- description: Content type for non-JSON documents (e.g., image/jpeg)
  name: mediaType
  type: string
- description: Content length in bytes for non-JSON documents
  name: bytes
  type: integer
provider_name: Oracle Database
provider_slug: oracle-database
schema_file: json-schema/oracle-database-document.json
slug: oracle-database-document
source_filename: oracle-database-document.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://oracle.com/schemas/database/document.json\",\n  \"title\": \"Oracle SODA Document\",\n  \"description\": \"Represents a JSON document stored in an Oracle SODA collection, including metadata such as key, version, and timestamps managed by the database.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique document key assigned by the server or client\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"Entity tag representing the document version for optimistic concurrency control\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last modification to the document\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the\
  \ document was created\"\n    },\n    \"value\": {\n      \"type\": \"object\",\n      \"description\": \"The JSON document content\"\n    },\n    \"mediaType\": {\n      \"type\": \"string\",\n      \"description\": \"Content type for non-JSON documents (e.g., image/jpeg)\",\n      \"default\": \"application/json\"\n    },\n    \"bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Content length in bytes for non-JSON documents\"\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-database/refs/heads/main/json-schema/oracle-database-document.json
tags:
- Cloud
- Database
- Enterprise
- Oracle
- REST API
- SQL
title: Oracle SODA Document
---
