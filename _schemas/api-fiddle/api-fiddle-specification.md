---
description: An API specification within an API Fiddle project, representing an OpenAPI document being designed or edited.
layout: schema
name: API Fiddle Specification
properties_list:
- description: Unique identifier for the specification.
  name: id
  type: string
- description: Identifier of the parent project.
  name: projectId
  type: string
- description: Name of the specification.
  name: name
  type: string
- description: A detailed description of the specification.
  name: description
  type: string
- description: Version label for the specification.
  name: version
  type: string
- description: The OpenAPI format version used by this specification.
  name: format
  type: string
- description: The raw specification content in YAML or JSON.
  name: content
  type: string
- description: Current lifecycle status of the specification.
  name: status
  type: string
- description: Timestamp when the specification was created.
  name: createdAt
  type: string
- description: Timestamp when the specification was last updated.
  name: updatedAt
  type: string
provider_name: API-Fiddle
provider_slug: api-fiddle
schema_file: json-schema/api-fiddle-specification-schema.json
slug: api-fiddle-specification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-fiddle.com/schemas/specification.json\",\n  \"title\": \"API Fiddle Specification\",\n  \"description\": \"An API specification within an API Fiddle project, representing an OpenAPI document being designed or edited.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the specification.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the parent project.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the specification.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of the specification.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version label for\
  \ the specification.\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\"openapi-3.0\", \"openapi-3.1\"],\n      \"description\": \"The OpenAPI format version used by this specification.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The raw specification content in YAML or JSON.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"draft\", \"review\", \"published\", \"archived\"],\n      \"description\": \"Current lifecycle status of the specification.\",\n      \"default\": \"draft\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the specification was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the specification was last updated.\"\n    }\n  },\n  \"required\": [\"id\", \"projectId\", \"name\"],\n  \"additionalProperties\"\
  : false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/api-fiddle/refs/heads/main/json-schema/api-fiddle-specification-schema.json
tags:
- API Design
- OpenAPI
- Collaboration
- Documentation
- Platform
title: API Fiddle Specification
---
