---
description: Schema representing an API entity (API definition) managed in the APIMatic platform
layout: schema
name: APIMatic API Entity
properties_list:
- description: Unique identifier of the API entity
  name: id
  type: string
- description: Name of the API
  name: name
  type: string
- description: Description of the API
  name: description
  type: string
- description: API version string
  name: version
  type: string
- description: Timestamp when the API entity was created
  name: createdAt
  type: string
- description: Timestamp when the API entity was last updated
  name: updatedAt
  type: string
provider_name: APIMatic
provider_slug: apimatic
schema_file: json-schema/apimatic-api-entity-schema.json
slug: apimatic-api-entity
source_filename: apimatic-api-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apimatic/main/json-schema/apimatic-api-entity-schema.json\",\n  \"title\": \"APIMatic API Entity\",\n  \"description\": \"Schema representing an API entity (API definition) managed in the APIMatic platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the API entity\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the API\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the API\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"API version string\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the API entity was created\"\n    },\n    \"updatedAt\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the API entity was last updated\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/json-schema/apimatic-api-entity-schema.json
tags:
- API Transformation
- Code Generation
- Developer Experience
- Documentation
- SDK Generation
title: APIMatic API Entity
---
