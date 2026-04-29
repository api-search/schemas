---
description: Schema for a schema object stored in Confluent Schema Registry.
layout: schema
name: Confluent Schema Registry Schema
properties_list:
- description: The subject the schema is registered under
  name: subject
  type: string
- description: Globally unique schema ID
  name: id
  type: integer
- description: Version number within the subject
  name: version
  type: integer
- description: The type of schema
  name: schemaType
  type: string
- description: The schema definition as a string
  name: schema
  type: string
- description: References to other schemas
  name: references
  type: array
- description: Compatibility level for this subject
  name: compatibilityLevel
  type: string
provider_name: Confluent Schema Registry
provider_slug: confluent-schema-registry
schema_file: json-schema/schema-registry-schema.json
slug: schema-registry
source_filename: schema-registry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/confluent-schema-registry/schema-registry-schema.json\",\n  \"title\": \"Confluent Schema Registry Schema\",\n  \"description\": \"Schema for a schema object stored in Confluent Schema Registry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject the schema is registered under\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Globally unique schema ID\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number within the subject\"\n    },\n    \"schemaType\": {\n      \"type\": \"string\",\n      \"enum\": [\"AVRO\", \"JSON\", \"PROTOBUF\"],\n      \"default\": \"AVRO\",\n      \"description\": \"The type of schema\"\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"The schema\
  \ definition as a string\"\n    },\n    \"references\": {\n      \"type\": \"array\",\n      \"description\": \"References to other schemas\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Reference name used in the schema\"\n          },\n          \"subject\": {\n            \"type\": \"string\",\n            \"description\": \"Subject of the referenced schema\"\n          },\n          \"version\": {\n            \"type\": \"integer\",\n            \"description\": \"Version of the referenced schema\"\n          }\n        },\n        \"required\": [\"name\", \"subject\", \"version\"]\n      }\n    },\n    \"compatibilityLevel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"BACKWARD\",\n        \"BACKWARD_TRANSITIVE\",\n        \"FORWARD\",\n        \"FORWARD_TRANSITIVE\",\n        \"FULL\",\n        \"FULL_TRANSITIVE\",\n        \"NONE\"\n      ],\n\
  \      \"description\": \"Compatibility level for this subject\"\n    }\n  },\n  \"required\": [\"schema\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluent-schema-registry/refs/heads/main/json-schema/schema-registry-schema.json
tags:
- Apache Kafka
- Avro
- Compatibility
- Confluent
- Data Governance
- Data Streaming
- JSON Schema
- Open Source
- Protobuf
- REST
- Schema Evolution
- Schema Registry
title: Confluent Schema Registry Schema
---
