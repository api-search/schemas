---
description: JSON Schema for Apollo Router and Federation supergraph configuration (supergraph.yaml / router.yaml).
layout: schema
name: Apollo Federation Supergraph Configuration
properties_list:
- description: Federation version for composition.
  name: federation_version
  type: string
- description: Subgraph definitions keyed by name.
  name: subgraphs
  type: object
provider_name: Apollo Federation
provider_slug: apollo-federation
schema_file: json-schema/supergraph-configuration.json
slug: supergraph-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/apollo-federation/json-schema/supergraph-configuration.json\",\n  \"title\": \"Apollo Federation Supergraph Configuration\",\n  \"description\": \"JSON Schema for Apollo Router and Federation supergraph configuration (supergraph.yaml / router.yaml).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"federation_version\": {\n      \"type\": \"string\",\n      \"enum\": [\"=2.0.0\", \"=2.3.0\", \"=2.5.0\", \"=2.6.0\", \"=2.7.0\", \"=2.8.0\", \"=2.9.0\"],\n      \"description\": \"Federation version for composition.\"\n    },\n    \"subgraphs\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/SubgraphConfig\"\n      },\n      \"description\": \"Subgraph definitions keyed by name.\"\n    }\n  },\n  \"$defs\": {\n    \"SubgraphConfig\": {\n      \"type\": \"object\",\n      \"required\": [\"routing_url\", \"schema\"\
  ],\n      \"properties\": {\n        \"routing_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL where the subgraph can be reached at runtime.\"\n        },\n        \"schema\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"file\": {\n              \"type\": \"string\",\n              \"description\": \"Path to the subgraph schema file.\"\n            },\n            \"subgraph_url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"URL to introspect the subgraph schema from.\"\n            },\n            \"graphref\": {\n              \"type\": \"string\",\n              \"description\": \"Apollo Studio graph reference (graph@variant).\"\n            }\n          },\n          \"description\": \"Subgraph schema source.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apollo-federation/refs/heads/main/json-schema/supergraph-configuration.json
tags:
- API Gateway
- Federation
- GraphQL
- Microservices
- Open Source
- Subgraphs
- Supergraph
title: Apollo Federation Supergraph Configuration
---
