---
description: An API definition within a project, including its generation source and lifecycle status.
layout: schema
name: APIGen API
properties_list:
- description: Unique identifier for the API.
  name: id
  type: string
- description: ID of the parent project.
  name: projectId
  type: string
- description: Human-readable name of the API.
  name: name
  type: string
- description: Detailed description of what the API does.
  name: description
  type: string
- description: Semantic version of the API.
  name: version
  type: string
- description: 'How the API was created: from a natural language prompt, an imported spec, or manually.'
  name: generationSource
  type: string
- description: The natural language prompt used to generate the API, if applicable.
  name: prompt
  type: string
- description: URL to the imported OpenAPI specification, if applicable.
  name: specUrl
  type: string
- description: Current lifecycle status of the API.
  name: status
  type: string
- description: Number of endpoints defined in this API.
  name: endpointCount
  type: integer
- description: Number of schemas defined in this API.
  name: schemaCount
  type: integer
- description: Tags for categorizing the API.
  name: tags
  type: array
- description: Timestamp when the API was created.
  name: createdAt
  type: string
- description: Timestamp when the API was last updated.
  name: updatedAt
  type: string
provider_name: APIGen
provider_slug: apigen
schema_file: json-schema/apigen-api-schema.json
slug: apigen-api
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.apigen.com/schemas/api.json\",\n  \"title\": \"APIGen API\",\n  \"description\": \"An API definition within a project, including its generation source and lifecycle status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the API.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"ID of the parent project.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 255,\n      \"description\": \"Human-readable name of the API.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of what the API does.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Semantic version\
  \ of the API.\"\n    },\n    \"generationSource\": {\n      \"type\": \"string\",\n      \"enum\": [\"prompt\", \"spec\", \"manual\"],\n      \"description\": \"How the API was created: from a natural language prompt, an imported spec, or manually.\"\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"The natural language prompt used to generate the API, if applicable.\"\n    },\n    \"specUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the imported OpenAPI specification, if applicable.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"draft\", \"generated\", \"published\"],\n      \"description\": \"Current lifecycle status of the API.\"\n    },\n    \"endpointCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of endpoints defined in this API.\"\n    },\n    \"schemaCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n \
  \     \"description\": \"Number of schemas defined in this API.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags for categorizing the API.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the API was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the API was last updated.\"\n    }\n  },\n  \"required\": [\"id\", \"projectId\", \"name\", \"version\", \"status\", \"createdAt\", \"updatedAt\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigen/refs/heads/main/json-schema/apigen-api-schema.json
tags:
- Code
- Documentation
- Generation
- Open Source
- PHP
title: APIGen API
---
