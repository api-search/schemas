---
description: Represents a semantic type registered in the Orbital workspace, used by TaxiQL to discover and orchestrate data fetching across connected services.
layout: schema
name: Orbital Type
properties_list:
- description: Fully qualified name of the type.
  name: qualifiedName
  type: string
- description: Kind of type definition.
  name: kind
  type: string
- description: Fields defined on this type (for MODEL types).
  name: fields
  type: array
- description: Data sources that expose this type.
  name: sources
  type: array
- description: ID of the schema that defines this type.
  name: schemaId
  type: string
provider_name: Orbital
provider_slug: orbital
schema_file: json-schema/type.json
slug: type
source_filename: type.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/json-schema/type.json\",\n  \"title\": \"Orbital Type\",\n  \"description\": \"Represents a semantic type registered in the Orbital workspace, used by TaxiQL to discover and orchestrate data fetching across connected services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"qualifiedName\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified name of the type.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Kind of type definition.\",\n      \"enum\": [\"SCALAR\", \"MODEL\", \"ENUM\", \"SERVICE\"]\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"Fields defined on this type (for MODEL types).\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n\
  \            \"description\": \"Field name.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Qualified type name of the field.\"\n          },\n          \"nullable\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the field is nullable.\"\n          }\n        }\n      }\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"description\": \"Data sources that expose this type.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"schemaId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the schema that defines this type.\"\n    }\n  },\n  \"required\": [\"qualifiedName\", \"kind\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/json-schema/type.json
tags:
- Data
- Gateways
title: Orbital Type
---
