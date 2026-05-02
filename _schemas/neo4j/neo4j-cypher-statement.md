---
description: A Cypher query statement with parameters for execution against a Neo4j database through the HTTP or Query API.
layout: schema
name: Neo4j Cypher Statement
properties_list:
- description: The Cypher query string to execute against the Neo4j database
  name: statement
  type: string
- description: Named parameters for the Cypher query. Always use parameters instead of string concatenation to protect against Cypher injection when incorporating user input.
  name: parameters
  type: object
- description: Requested result formats for the HTTP API. Possible values include row for tabular data and graph for graph visualization data.
  name: resultDataContents
  type: array
- description: Whether to include query execution statistics such as nodes created, relationships created, and properties set in the response.
  name: includeStats
  type: boolean
provider_name: Neo4j
provider_slug: neo4j
schema_file: json-schema/neo4j-cypher-statement-schema.json
slug: neo4j-cypher-statement
source_filename: neo4j-cypher-statement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://neo4j.com/schemas/neo4j/cypher-statement.json\",\n  \"title\": \"Neo4j Cypher Statement\",\n  \"description\": \"A Cypher query statement with parameters for execution against a Neo4j database through the HTTP or Query API.\",\n  \"type\": \"object\",\n  \"required\": [\"statement\"],\n  \"properties\": {\n    \"statement\": {\n      \"type\": \"string\",\n      \"description\": \"The Cypher query string to execute against the Neo4j database\",\n      \"minLength\": 1,\n      \"examples\": [\n        \"MATCH (n:Person {name: $name}) RETURN n\",\n        \"CREATE (n:Person {name: $name, age: $age}) RETURN n\"\n      ]\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Named parameters for the Cypher query. Always use parameters instead of string concatenation to protect against Cypher injection when incorporating user input.\",\n      \"additionalProperties\"\
  : true,\n      \"examples\": [\n        {\n          \"name\": \"Alice\",\n          \"age\": 30\n        }\n      ]\n    },\n    \"resultDataContents\": {\n      \"type\": \"array\",\n      \"description\": \"Requested result formats for the HTTP API. Possible values include row for tabular data and graph for graph visualization data.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"row\", \"graph\"]\n      },\n      \"uniqueItems\": true\n    },\n    \"includeStats\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include query execution statistics such as nodes created, relationships created, and properties set in the response.\",\n      \"default\": false\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/neo4j/refs/heads/main/json-schema/neo4j-cypher-statement-schema.json
tags:
- Graph Database
- Cypher
- Cloud
- GraphQL
- Drivers
- APIs
title: Neo4j Cypher Statement
---
