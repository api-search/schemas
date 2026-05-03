---
description: A catalog entity instance in the Rely.io software catalog
layout: schema
name: Rely.io Entity
properties_list:
- description: Unique entity identifier
  name: id
  type: string
- description: The blueprint type this entity is an instance of
  name: blueprintId
  type: string
- description: Entity display name
  name: name
  type: string
- description: Property values conforming to the blueprint's property schema
  name: properties
  type: object
- description: Related entity identifiers keyed by relation name
  name: relations
  type: object
- description: Entity creation timestamp
  name: createdAt
  type: string
- description: Entity last update timestamp
  name: updatedAt
  type: string
provider_name: Rely.io
provider_slug: rely
schema_file: json-schema/rely-entity-schema.json
slug: rely-entity
source_filename: rely-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://api-evangelist.github.io/rely/json-schema/rely-entity-schema.json\",\n  \"title\": \"Rely.io Entity\",\n  \"description\": \"A catalog entity instance in the Rely.io software catalog\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"blueprintId\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique entity identifier\"\n    },\n    \"blueprintId\": {\n      \"type\": \"string\",\n      \"description\": \"The blueprint type this entity is an instance of\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Entity display name\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Property values conforming to the blueprint's property schema\",\n      \"additionalProperties\": true\n    },\n    \"relations\": {\n      \"type\": \"object\",\n      \"description\": \"Related\
  \ entity identifiers keyed by relation name\",\n      \"additionalProperties\": {\n        \"oneOf\": [\n          { \"type\": \"string\" },\n          { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n          { \"type\": \"null\" }\n        ]\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Entity creation timestamp\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Entity last update timestamp\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rely/refs/heads/main/json-schema/rely-entity-schema.json
tags:
- Developer Experience
- Internal Developer Portal
- Platform Engineering
- Software Catalog
- Service Catalog
- Engineering Scorecards
title: Rely.io Entity
---
