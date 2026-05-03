---
description: Represents a schema registered in the Orbital workspace, containing type definitions from API specs, database schemas, or Taxi projects.
layout: schema
name: Orbital Schema
properties_list:
- description: Unique identifier for the schema.
  name: id
  type: string
- description: Human-readable name of the schema.
  name: name
  type: string
- description: Version of the schema.
  name: version
  type: string
- description: Source format of the schema.
  name: source
  type: string
- description: The raw schema content.
  name: content
  type: string
- description: Types defined in this schema.
  name: types
  type: array
- description: Timestamp when the schema was registered.
  name: createdAt
  type: string
- description: Timestamp when the schema was last updated.
  name: updatedAt
  type: string
provider_name: Orbital
provider_slug: orbital
schema_file: json-schema/schema.json
slug: schema
source_filename: schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/json-schema/schema.json\",\n  \"title\": \"Orbital Schema\",\n  \"description\": \"Represents a schema registered in the Orbital workspace, containing type definitions from API specs, database schemas, or Taxi projects.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the schema.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the schema.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the schema.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source format of the schema.\",\n      \"enum\": [\"TAXI\", \"OPEN_API\", \"PROTOBUF\", \"AVRO\", \"JSON_SCHEMA\", \"DATABASE\"]\n    },\n    \"content\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The raw schema content.\"\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"Types defined in this schema.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the schema was registered.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the schema was last updated.\"\n    }\n  },\n  \"required\": [\"name\", \"source\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/json-schema/schema.json
tags:
- Data
- Gateways
title: Orbital Schema
---
