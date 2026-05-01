---
description: Represents a document in a Fauna collection. Documents are the primary data unit in Fauna and consist of fields with values. Each document belongs to a collection and has a unique reference identifier, creation timestamp, and transaction timestamp.
layout: schema
name: Fauna Document
properties_list:
- description: Unique identifier for the document within its collection.
  name: id
  type: string
- description: The name of the collection this document belongs to.
  name: coll
  type: string
- description: Transaction timestamp in microseconds since the Unix epoch representing the last time this document was modified.
  name: ts
  type: integer
- description: The user-defined fields and values stored in this document. Field names and types are defined by the collection schema.
  name: data
  type: object
provider_name: fauna
provider_slug: fauna
schema_file: json-schema/fauna-document-schema.json
slug: fauna-document
source_filename: fauna-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://fauna.com/schemas/fauna/document.json\",\n  \"title\": \"Fauna Document\",\n  \"description\": \"Represents a document in a Fauna collection. Documents are the primary data unit in Fauna and consist of fields with values. Each document belongs to a collection and has a unique reference identifier, creation timestamp, and transaction timestamp.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"coll\", \"ts\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the document within its collection.\"\n    },\n    \"coll\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the collection this document belongs to.\"\n    },\n    \"ts\": {\n      \"type\": \"integer\",\n      \"description\": \"Transaction timestamp in microseconds since the Unix epoch representing the last time this document was modified.\"\
  \n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"The user-defined fields and values stored in this document. Field names and types are defined by the collection schema.\"\n    }\n  },\n  \"additionalProperties\": true,\n  \"$defs\": {\n    \"DocumentReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a Fauna document by its collection and ID.\",\n      \"required\": [\"id\", \"coll\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the referenced document.\"\n        },\n        \"coll\": {\n          \"type\": \"string\",\n          \"description\": \"Collection name of the referenced document.\"\n        }\n      }\n    },\n    \"NamedDocument\": {\n      \"type\": \"object\",\n      \"description\": \"A system document referenced by name rather than ID, such as collections, indexes, and roles.\",\n  \
  \    \"required\": [\"name\", \"coll\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The unique name of the system document.\"\n        },\n        \"coll\": {\n          \"type\": \"string\",\n          \"description\": \"The system collection this document belongs to, such as Collection, Index, or Role.\"\n        },\n        \"ts\": {\n          \"type\": \"integer\",\n          \"description\": \"Transaction timestamp of the last modification.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fauna/refs/heads/main/json-schema/fauna-document-schema.json
tags: []
title: Fauna Document
---
