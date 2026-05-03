---
description: Minimal schema for describing a RESTful API — its identity, endpoints, and interface characteristics.
layout: schema
name: RESTful API Description
properties_list:
- description: Unique identifier for this API
  name: id
  type: string
- description: Human-readable API name
  name: name
  type: string
- description: What the API does and who it is for
  name: description
  type: string
- description: API version (e.g., 1.0, v2, 2026-05-01)
  name: version
  type: string
- description: Base URL for all API endpoints
  name: baseUrl
  type: string
- description: URL of the human-readable API documentation
  name: documentationUrl
  type: string
- description: URL of the machine-readable OpenAPI specification
  name: specificationUrl
  type: string
- description: Authentication requirements
  name: authentication
  type: object
- description: Richardson Maturity Model level (0-3)
  name: maturityLevel
  type: integer
- description: Domain tags for classification
  name: tags
  type: array
provider_name: RESTful
provider_slug: restful
schema_file: json-schema/restful-api-description-schema.json
slug: restful-api-description
source_filename: restful-api-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/restful/schemas/api-description\",\n  \"title\": \"RESTful API Description\",\n  \"description\": \"Minimal schema for describing a RESTful API — its identity, endpoints, and interface characteristics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this API\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable API name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"What the API does and who it is for\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"API version (e.g., 1.0, v2, 2026-05-01)\"\n    },\n    \"baseUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Base URL for all API endpoints\"\n    },\n    \"documentationUrl\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the human-readable API documentation\"\n    },\n    \"specificationUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the machine-readable OpenAPI specification\"\n    },\n    \"authentication\": {\n      \"type\": \"object\",\n      \"description\": \"Authentication requirements\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"none\", \"apiKey\", \"bearer\", \"basic\", \"oauth2\", \"openid\"],\n          \"description\": \"Authentication scheme\"\n        },\n        \"documentationUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Authentication setup documentation\"\n        }\n      }\n    },\n    \"maturityLevel\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 3,\n      \"description\": \"Richardson Maturity\
  \ Model level (0-3)\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Domain tags for classification\"\n    }\n  },\n  \"required\": [\"name\", \"baseUrl\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/restful/refs/heads/main/json-schema/restful-api-description-schema.json
tags:
- Architecture
- HTTP
- Web Services
title: RESTful API Description
---
