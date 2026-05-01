---
description: An entity from the Google Knowledge Graph.
layout: schema
name: Google Knowledge Graph Entity
properties_list:
- description: The canonical URI for the entity.
  name: '@id'
  type: string
- description: The name of the entity.
  name: name
  type: string
- description: The schema.org types of the entity.
  name: '@type'
  type: array
- description: A short description of the entity.
  name: description
  type: string
- description: An image associated with the entity.
  name: image
  type: object
- description: A detailed description of the entity.
  name: detailedDescription
  type: object
- description: The official website URL for the entity.
  name: url
  type: string
provider_name: Google Knowledge Graph Search
provider_slug: google-knowledge-graph
schema_file: json-schema/Entity.json
slug: Entity
source_filename: Entity.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"Entity.json\",\n  \"title\": \"Google Knowledge Graph Entity\",\n  \"description\": \"An entity from the Google Knowledge Graph.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@id\": {\n      \"type\": \"string\",\n      \"description\": \"The canonical URI for the entity.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the entity.\"\n    },\n    \"@type\": {\n      \"type\": \"array\",\n      \"description\": \"The schema.org types of the entity.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A short description of the entity.\"\n    },\n    \"image\": {\n      \"type\": \"object\",\n      \"description\": \"An image associated with the entity.\",\n      \"properties\": {\n        \"contentUrl\": {\n          \"type\": \"string\",\n     \
  \     \"format\": \"uri\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      }\n    },\n    \"detailedDescription\": {\n      \"type\": \"object\",\n      \"description\": \"A detailed description of the entity.\",\n      \"properties\": {\n        \"articleBody\": {\n          \"type\": \"string\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"license\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      }\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The official website URL for the entity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-knowledge-graph/refs/heads/main/json-schema/Entity.json
tags:
- Entities
- Google
- Knowledge Graph
- Linked Data
- Schema.org
- Semantic Search
title: Google Knowledge Graph Entity
---
