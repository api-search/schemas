---
description: ExecuteOpenCypherExplainInput schema from Neptune
layout: schema
name: ExecuteOpenCypherExplainInput
properties_list:
- description: The openCypher query to explain.
  name: query
  type: string
- description: ''
  name: parameters
  type: string
- description: The explain mode (static, dynamic, or details).
  name: explainMode
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-execute-open-cypher-explain-input-schema.json
slug: data-execute-open-cypher-explain-input
source_filename: data-execute-open-cypher-explain-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-execute-open-cypher-explain-input-schema.json\",\n  \"title\": \"ExecuteOpenCypherExplainInput\",\n  \"description\": \"ExecuteOpenCypherExplainInput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"The openCypher query to explain.\"\n    },\n    \"parameters\": {\n      \"type\": \"string\"\n    },\n    \"explainMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"static\",\n        \"dynamic\",\n        \"details\"\n      ],\n      \"description\": \"The explain mode (static, dynamic, or details).\"\n    }\n  },\n  \"required\": [\n    \"query\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-execute-open-cypher-explain-input-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: ExecuteOpenCypherExplainInput
---
