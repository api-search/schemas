---
description: A Federated Graph represents the composed supergraph made up of multiple subgraphs selected by label matchers in the WunderGraph Cosmo platform.
layout: schema
name: WunderGraph Cosmo Federated Graph
properties_list:
- description: Unique identifier for the federated graph.
  name: id
  type: string
- description: The name of the federated graph.
  name: name
  type: string
- description: The namespace the graph belongs to.
  name: namespace
  type: string
- description: The URL where the router is hosted.
  name: routingUrl
  type: string
- description: Label matchers used to select subgraphs for composition (e.g., team=backend).
  name: labelMatchers
  type: array
- description: The current composition status of the graph.
  name: compositionStatus
  type: string
- description: When the graph was last successfully composed.
  name: lastComposedAt
  type: string
- description: Number of subgraphs composing the federated graph.
  name: subgraphsCount
  type: integer
- description: Readme description of the graph.
  name: readme
  type: string
- description: When the federated graph was created.
  name: createdAt
  type: string
- description: When the federated graph was last updated.
  name: updatedAt
  type: string
provider_name: WunderGraph
provider_slug: wundergraph
schema_file: json-schema/federated-graph.json
slug: federated-graph
source_filename: federated-graph.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/wundergraph/blob/main/json-schema/federated-graph.json\",\n  \"title\": \"WunderGraph Cosmo Federated Graph\",\n  \"description\": \"A Federated Graph represents the composed supergraph made up of multiple subgraphs selected by label matchers in the WunderGraph Cosmo platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the federated graph.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the federated graph.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace the graph belongs to.\"\n    },\n    \"routingUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL where the router is hosted.\"\n    },\n    \"labelMatchers\": {\n    \
  \  \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Label matchers used to select subgraphs for composition (e.g., team=backend).\"\n    },\n    \"compositionStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"SUCCESS\", \"FAILURE\", \"PENDING\"],\n      \"description\": \"The current composition status of the graph.\"\n    },\n    \"lastComposedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the graph was last successfully composed.\"\n    },\n    \"subgraphsCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of subgraphs composing the federated graph.\"\n    },\n    \"readme\": {\n      \"type\": \"string\",\n      \"description\": \"Readme description of the graph.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the federated graph was created.\"\n    },\n    \"updatedAt\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the federated graph was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/json-schema/federated-graph.json
tags:
- Federation
- GraphQL
- Management
- Schema Registry
title: WunderGraph Cosmo Federated Graph
---
