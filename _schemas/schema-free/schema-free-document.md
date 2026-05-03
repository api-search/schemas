---
description: Represents a document in a schema-free (schemaless) database. Only minimal metadata fields are required; all other content is flexible and application-defined.
layout: schema
name: Schema-Free Document
properties_list:
- description: Unique identifier for the document (auto-assigned or application-provided)
  name: _id
  type: string
- description: Collection or table name this document belongs to
  name: _collection
  type: string
- description: Optimistic concurrency version number for the document
  name: _version
  type: integer
- description: Timestamp when the document was first created
  name: _created
  type: string
- description: Timestamp when the document was last modified
  name: _modified
  type: string
- description: Application-level document type discriminator (e.g., 'user', 'order', 'product')
  name: _type
  type: string
provider_name: Schema Free
provider_slug: schema-free
schema_file: json-schema/schema-free-document-schema.json
slug: schema-free-document
source_filename: schema-free-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://github.com/api-evangelist/schema-free/blob/main/json-schema/schema-free-document-schema.json\",\n  \"title\": \"Schema-Free Document\",\n  \"description\": \"Represents a document in a schema-free (schemaless) database. Only minimal metadata fields are required; all other content is flexible and application-defined.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the document (auto-assigned or application-provided)\"\n    },\n    \"_collection\": {\n      \"type\": \"string\",\n      \"description\": \"Collection or table name this document belongs to\"\n    },\n    \"_version\": {\n      \"type\": \"integer\",\n      \"description\": \"Optimistic concurrency version number for the document\",\n      \"minimum\": 1\n    },\n    \"_created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"Timestamp when the document was first created\"\n    },\n    \"_modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the document was last modified\"\n    },\n    \"_type\": {\n      \"type\": \"string\",\n      \"description\": \"Application-level document type discriminator (e.g., 'user', 'order', 'product')\"\n    }\n  },\n  \"additionalProperties\": true,\n  \"description_notes\": \"The additionalProperties: true setting reflects the schemaless nature of these databases — any additional fields are valid. Application-level validation handles field constraints.\",\n  \"examples\": [\n    {\n      \"_id\": \"64f8c9d12a3e4b5c6d7e8f90\",\n      \"_collection\": \"products\",\n      \"_version\": 3,\n      \"_created\": \"2026-01-15T09:00:00Z\",\n      \"_modified\": \"2026-05-01T14:30:00Z\",\n      \"_type\": \"physical-product\",\n      \"name\": \"Zebra ZD421 Label Printer\",\n      \"sku\": \"\
  ZD42143-D0E000EZ\",\n      \"price\": 249.99,\n      \"tags\": [\"barcode\", \"thermal\", \"desktop\"],\n      \"specs\": {\n        \"resolution\": \"203 dpi\",\n        \"maxPrintWidth\": 4.09,\n        \"interfaces\": [\"USB\", \"Ethernet\", \"Bluetooth\"]\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-free/refs/heads/main/json-schema/schema-free-document-schema.json
tags:
- Schema Free
- Schemaless
- NoSQL
- Document Store
- Flexible Schema
- MongoDB
- DynamoDB
- Elasticsearch
title: Schema-Free Document
---
