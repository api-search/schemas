---
description: A property graph relationship as returned by openCypher queries.
layout: schema
name: OpenCypherRelationship
properties_list:
- description: The unique identifier of the relationship.
  name: ~id
  type: string
- description: The entity type (always 'relationship').
  name: ~entityType
  type: string
- description: The ID of the source node.
  name: ~start
  type: string
- description: The ID of the target node.
  name: ~end
  type: string
- description: The relationship type.
  name: ~type
  type: string
- description: The relationship properties as key-value pairs.
  name: ~properties
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/opencypher-open-cypher-relationship-schema.json
slug: opencypher-open-cypher-relationship
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/opencypher-open-cypher-relationship-schema.json\",\n  \"title\": \"OpenCypherRelationship\",\n  \"description\": \"A property graph relationship as returned by openCypher queries.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"~id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the relationship.\"\n    },\n    \"~entityType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"relationship\"\n      ],\n      \"description\": \"The entity type (always 'relationship').\"\n    },\n    \"~start\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the source node.\"\n    },\n    \"~end\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the target node.\"\n    },\n    \"~type\": {\n      \"type\": \"string\",\n      \"\
  description\": \"The relationship type.\"\n    },\n    \"~properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"The relationship properties as key-value pairs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/opencypher-open-cypher-relationship-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: OpenCypherRelationship
---
