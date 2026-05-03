---
description: Represents a schema definition used in API design — a formal description of the structure and constraints of a data type used in requests, responses, or events.
layout: schema
name: API Schema Definition
properties_list:
- description: Human-readable name for this schema
  name: name
  type: string
- description: Schema format or specification
  name: format
  type: string
- description: Schema version identifier
  name: version
  type: string
- description: Description of what this schema represents
  name: description
  type: string
- description: List of field definitions in this schema
  name: fields
  type: array
- description: Validation constraints applied to the schema
  name: constraints
  type: object
- description: Example instances conforming to this schema
  name: examples
  type: array
- description: Classification tags for this schema
  name: tags
  type: array
- description: Date the schema was created
  name: created
  type: string
- description: Date the schema was last modified
  name: modified
  type: string
provider_name: Schema Design
provider_slug: schema-design
schema_file: json-schema/schema-design-api-schema-schema.json
slug: schema-design-api-schema
source_filename: schema-design-api-schema-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://github.com/api-evangelist/schema-design/blob/main/json-schema/schema-design-api-schema-schema.json\",\n  \"title\": \"API Schema Definition\",\n  \"description\": \"Represents a schema definition used in API design — a formal description of the structure and constraints of a data type used in requests, responses, or events.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for this schema\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"Schema format or specification\",\n      \"enum\": [\"json-schema\", \"openapi\", \"graphql\", \"avro\", \"protobuf\", \"xsd\", \"thrift\"]\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Schema version identifier\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"Description of what this schema represents\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"List of field definitions in this schema\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\" },\n          \"type\": { \"type\": \"string\" },\n          \"required\": { \"type\": \"boolean\" },\n          \"description\": { \"type\": \"string\" },\n          \"format\": { \"type\": \"string\" },\n          \"enum\": {\n            \"type\": \"array\",\n            \"items\": { \"type\": \"string\" }\n          },\n          \"default\": {}\n        },\n        \"required\": [\"name\", \"type\"]\n      }\n    },\n    \"constraints\": {\n      \"type\": \"object\",\n      \"description\": \"Validation constraints applied to the schema\",\n      \"properties\": {\n        \"required\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\"\
  : \"List of required field names\"\n        },\n        \"additionalProperties\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether additional undeclared properties are allowed\"\n        }\n      }\n    },\n    \"examples\": {\n      \"type\": \"array\",\n      \"description\": \"Example instances conforming to this schema\",\n      \"items\": { \"type\": \"object\" }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Classification tags for this schema\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the schema was created\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the schema was last modified\"\n    }\n  },\n  \"required\": [\"name\", \"format\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-design/refs/heads/main/json-schema/schema-design-api-schema-schema.json
tags:
- Schema Design
- Data Modeling
- API Design
- JSON Schema
- OpenAPI
- GraphQL
- Data Validation
- Type Systems
title: API Schema Definition
---
