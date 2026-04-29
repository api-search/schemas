---
description: A property graph node as returned by openCypher queries.
layout: schema
name: OpenCypherNode
properties_list:
- description: The unique identifier of the node.
  name: ~id
  type: string
- description: The entity type (always 'node').
  name: ~entityType
  type: string
- description: The labels assigned to the node.
  name: ~labels
  type: array
- description: The node properties as key-value pairs.
  name: ~properties
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/opencypher-open-cypher-node-schema.json
slug: opencypher-open-cypher-node
source_filename: opencypher-open-cypher-node-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/opencypher-open-cypher-node-schema.json\",\n  \"title\": \"OpenCypherNode\",\n  \"description\": \"A property graph node as returned by openCypher queries.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"~id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the node.\"\n    },\n    \"~entityType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"node\"\n      ],\n      \"description\": \"The entity type (always 'node').\"\n    },\n    \"~labels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The labels assigned to the node.\"\n    },\n    \"~properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"The node properties as key-value\
  \ pairs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/opencypher-open-cypher-node-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: OpenCypherNode
---
