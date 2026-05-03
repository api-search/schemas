---
description: A Feature Flag enables gradual rollout of feature subgraphs to federated graphs in the WunderGraph Cosmo platform.
layout: schema
name: WunderGraph Cosmo Feature Flag
properties_list:
- description: Unique identifier for the feature flag.
  name: id
  type: string
- description: The name of the feature flag.
  name: name
  type: string
- description: The namespace the feature flag belongs to.
  name: namespace
  type: string
- description: Whether the feature flag is currently enabled.
  name: isEnabled
  type: boolean
- description: Associated feature subgraph names.
  name: featureSubgraphNames
  type: array
- description: Labels to match federated graphs.
  name: labels
  type: array
- description: When the feature flag was created.
  name: createdAt
  type: string
- description: When the feature flag was last updated.
  name: updatedAt
  type: string
provider_name: WunderGraph
provider_slug: wundergraph
schema_file: json-schema/feature-flag.json
slug: feature-flag
source_filename: feature-flag.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/wundergraph/blob/main/json-schema/feature-flag.json\",\n  \"title\": \"WunderGraph Cosmo Feature Flag\",\n  \"description\": \"A Feature Flag enables gradual rollout of feature subgraphs to federated graphs in the WunderGraph Cosmo platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the feature flag.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the feature flag.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace the feature flag belongs to.\"\n    },\n    \"isEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the feature flag is currently enabled.\"\n    },\n    \"featureSubgraphNames\": {\n      \"type\": \"array\",\n      \"items\": {\n \
  \       \"type\": \"string\"\n      },\n      \"description\": \"Associated feature subgraph names.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"description\": \"Labels to match federated graphs.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the feature flag was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the feature flag was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/json-schema/feature-flag.json
tags:
- Federation
- GraphQL
- Management
- Schema Registry
title: WunderGraph Cosmo Feature Flag
---
