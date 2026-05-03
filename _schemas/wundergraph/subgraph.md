---
description: A Subgraph is an isolated GraphQL schema that can be independently deployed and managed, composing into federated graphs via label matching.
layout: schema
name: WunderGraph Cosmo Subgraph
properties_list:
- description: Unique identifier for the subgraph.
  name: id
  type: string
- description: The name of the subgraph.
  name: name
  type: string
- description: The namespace the subgraph belongs to.
  name: namespace
  type: string
- description: The URL where the subgraph service is hosted.
  name: routingUrl
  type: string
- description: Labels attached to the subgraph for matching to federated graphs.
  name: labels
  type: array
- description: URL for WebSocket-based GraphQL subscriptions if different from the routing URL.
  name: subscriptionUrl
  type: string
- description: The subscription transport protocol.
  name: subscriptionProtocol
  type: string
- description: When the schema was last published.
  name: lastPublishedAt
  type: string
- description: Readme description of the subgraph.
  name: readme
  type: string
- description: When the subgraph was created.
  name: createdAt
  type: string
- description: When the subgraph was last updated.
  name: updatedAt
  type: string
provider_name: WunderGraph
provider_slug: wundergraph
schema_file: json-schema/subgraph.json
slug: subgraph
source_filename: subgraph.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/wundergraph/blob/main/json-schema/subgraph.json\",\n  \"title\": \"WunderGraph Cosmo Subgraph\",\n  \"description\": \"A Subgraph is an isolated GraphQL schema that can be independently deployed and managed, composing into federated graphs via label matching.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the subgraph.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the subgraph.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace the subgraph belongs to.\"\n    },\n    \"routingUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL where the subgraph service is hosted.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n  \
  \    \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"description\": \"Labels attached to the subgraph for matching to federated graphs.\"\n    },\n    \"subscriptionUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for WebSocket-based GraphQL subscriptions if different from the routing URL.\"\n    },\n    \"subscriptionProtocol\": {\n      \"type\": \"string\",\n      \"enum\": [\"ws\", \"sse\", \"sse_post\"],\n      \"description\": \"The subscription transport protocol.\"\n    },\n    \"lastPublishedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the schema was last published.\"\n    },\n    \"readme\": {\n      \"type\": \"string\",\n      \"description\": \"Readme description of the subgraph.\"\
  \n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the subgraph was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the subgraph was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/json-schema/subgraph.json
tags:
- Federation
- GraphQL
- Management
- Schema Registry
title: WunderGraph Cosmo Subgraph
---
