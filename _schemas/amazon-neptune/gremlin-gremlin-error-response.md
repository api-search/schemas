---
description: GremlinErrorResponse schema from Neptune
layout: schema
name: GremlinErrorResponse
properties_list:
- description: ''
  name: requestId
  type: string
- description: The error code.
  name: code
  type: string
- description: A detailed description of the error.
  name: detailedMessage
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/gremlin-gremlin-error-response-schema.json
slug: gremlin-gremlin-error-response
source_filename: gremlin-gremlin-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/gremlin-gremlin-error-response-schema.json\",\n  \"title\": \"GremlinErrorResponse\",\n  \"description\": \"GremlinErrorResponse schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The error code.\"\n    },\n    \"detailedMessage\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/gremlin-gremlin-error-response-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: GremlinErrorResponse
---
