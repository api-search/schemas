---
description: A Monograph is a non-federated graph limited to a single subgraph, with GraphQL Federation disabled.
layout: schema
name: WunderGraph Cosmo Monograph
properties_list:
- description: Unique identifier for the monograph.
  name: id
  type: string
- description: The name of the monograph.
  name: name
  type: string
- description: The namespace the monograph belongs to.
  name: namespace
  type: string
- description: The URL where the router is hosted.
  name: routingUrl
  type: string
- description: The URL of the GraphQL service.
  name: graphUrl
  type: string
- description: The current composition status of the monograph.
  name: compositionStatus
  type: string
- description: Readme description of the monograph.
  name: readme
  type: string
- description: When the monograph was created.
  name: createdAt
  type: string
- description: When the monograph was last updated.
  name: updatedAt
  type: string
provider_name: WunderGraph
provider_slug: wundergraph
schema_file: json-schema/monograph.json
slug: monograph
source_filename: monograph.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/wundergraph/blob/main/json-schema/monograph.json\",\n  \"title\": \"WunderGraph Cosmo Monograph\",\n  \"description\": \"A Monograph is a non-federated graph limited to a single subgraph, with GraphQL Federation disabled.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the monograph.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the monograph.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace the monograph belongs to.\"\n    },\n    \"routingUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL where the router is hosted.\"\n    },\n    \"graphUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\"\
  : \"The URL of the GraphQL service.\"\n    },\n    \"compositionStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"SUCCESS\", \"FAILURE\", \"PENDING\"],\n      \"description\": \"The current composition status of the monograph.\"\n    },\n    \"readme\": {\n      \"type\": \"string\",\n      \"description\": \"Readme description of the monograph.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the monograph was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the monograph was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/json-schema/monograph.json
tags:
- Federation
- GraphQL
- Management
- Schema Registry
title: WunderGraph Cosmo Monograph
---
