---
description: Abstract schema for a RESTful API resource, defining the common structural pattern of a REST resource with identifier, metadata, and links.
layout: schema
name: REST Resource
properties_list:
- description: Unique resource identifier
  name: id
  type:
  - string
  - integer
- description: Resource type name (e.g., user, order, product)
  name: type
  type: string
- description: 'Self-link: the canonical URL for this resource'
  name: href
  type: string
- description: ISO 8601 creation timestamp
  name: createdAt
  type: string
- description: ISO 8601 last modification timestamp
  name: updatedAt
  type: string
- description: Hypermedia links (HAL-style) to related resources and available actions
  name: _links
  type: object
provider_name: RESTful Services
provider_slug: restful-services
schema_file: json-schema/restful-services-resource-schema.json
slug: restful-services-resource
source_filename: restful-services-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/restful-services/schemas/rest-resource\",\n  \"title\": \"REST Resource\",\n  \"description\": \"Abstract schema for a RESTful API resource, defining the common structural pattern of a REST resource with identifier, metadata, and links.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": [\"string\", \"integer\"],\n      \"description\": \"Unique resource identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type name (e.g., user, order, product)\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Self-link: the canonical URL for this resource\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 creation timestamp\"\n    },\n    \"updatedAt\": {\n     \
  \ \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 last modification timestamp\"\n    },\n    \"_links\": {\n      \"type\": \"object\",\n      \"description\": \"Hypermedia links (HAL-style) to related resources and available actions\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"href\": { \"type\": \"string\", \"format\": \"uri\" },\n          \"method\": { \"type\": \"string\", \"enum\": [\"GET\", \"POST\", \"PUT\", \"DELETE\", \"PATCH\"] },\n          \"title\": { \"type\": \"string\" }\n        }\n      }\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/restful-services/refs/heads/main/json-schema/restful-services-resource-schema.json
tags:
- Architecture
- HTTP
- Microservices
- REST
- Web Services
title: REST Resource
---
