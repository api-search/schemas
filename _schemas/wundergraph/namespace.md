---
description: A Namespace provides logical isolation for federated graphs, subgraphs, and other resources within the WunderGraph Cosmo platform.
layout: schema
name: WunderGraph Cosmo Namespace
properties_list:
- description: Unique identifier for the namespace.
  name: id
  type: string
- description: The name of the namespace.
  name: name
  type: string
- description: When the namespace was created.
  name: createdAt
  type: string
provider_name: WunderGraph
provider_slug: wundergraph
schema_file: json-schema/namespace.json
slug: namespace
source_filename: namespace.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/wundergraph/blob/main/json-schema/namespace.json\",\n  \"title\": \"WunderGraph Cosmo Namespace\",\n  \"description\": \"A Namespace provides logical isolation for federated graphs, subgraphs, and other resources within the WunderGraph Cosmo platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the namespace.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the namespace.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the namespace was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/json-schema/namespace.json
tags:
- Federation
- GraphQL
- Management
- Schema Registry
title: WunderGraph Cosmo Namespace
---
