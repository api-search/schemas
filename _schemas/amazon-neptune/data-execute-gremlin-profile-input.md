---
description: ExecuteGremlinProfileInput schema from Neptune
layout: schema
name: ExecuteGremlinProfileInput
properties_list:
- description: The Gremlin traversal query string to profile.
  name: gremlin
  type: string
- description: Whether to include results in the profile output.
  name: results
  type: boolean
- description: Maximum length of result string per entry.
  name: chop
  type: integer
- description: The serialization format for results.
  name: serializer
  type: string
- description: Whether to include index operation details.
  name: indexOps
  type: boolean
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-execute-gremlin-profile-input-schema.json
slug: data-execute-gremlin-profile-input
source_filename: data-execute-gremlin-profile-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-execute-gremlin-profile-input-schema.json\",\n  \"title\": \"ExecuteGremlinProfileInput\",\n  \"description\": \"ExecuteGremlinProfileInput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gremlin\": {\n      \"type\": \"string\",\n      \"description\": \"The Gremlin traversal query string to profile.\"\n    },\n    \"results\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include results in the profile output.\"\n    },\n    \"chop\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum length of result string per entry.\"\n    },\n    \"serializer\": {\n      \"type\": \"string\",\n      \"description\": \"The serialization format for results.\"\n    },\n    \"indexOps\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ to include index operation details.\"\n    }\n  },\n  \"required\": [\n    \"gremlin\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-execute-gremlin-profile-input-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: ExecuteGremlinProfileInput
---
