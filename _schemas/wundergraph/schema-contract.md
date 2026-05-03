---
description: A Schema Contract provides a filtered version of a composed federated graph to different consumers based on tag exclusions.
layout: schema
name: WunderGraph Cosmo Schema Contract
properties_list:
- description: Unique identifier for the contract.
  name: id
  type: string
- description: The name of the contract.
  name: name
  type: string
- description: The namespace the contract belongs to.
  name: namespace
  type: string
- description: The source federated graph.
  name: sourceGraphName
  type: string
- description: The routing URL for the contract graph.
  name: routingUrl
  type: string
- description: Tags excluded from the contract schema.
  name: excludeTags
  type: array
- description: The current composition status of the contract.
  name: compositionStatus
  type: string
- description: When the contract was created.
  name: createdAt
  type: string
- description: When the contract was last updated.
  name: updatedAt
  type: string
provider_name: WunderGraph
provider_slug: wundergraph
schema_file: json-schema/schema-contract.json
slug: schema-contract
source_filename: schema-contract.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/wundergraph/blob/main/json-schema/schema-contract.json\",\n  \"title\": \"WunderGraph Cosmo Schema Contract\",\n  \"description\": \"A Schema Contract provides a filtered version of a composed federated graph to different consumers based on tag exclusions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the contract.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the contract.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace the contract belongs to.\"\n    },\n    \"sourceGraphName\": {\n      \"type\": \"string\",\n      \"description\": \"The source federated graph.\"\n    },\n    \"routingUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\"\
  : \"The routing URL for the contract graph.\"\n    },\n    \"excludeTags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags excluded from the contract schema.\"\n    },\n    \"compositionStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"SUCCESS\", \"FAILURE\", \"PENDING\"],\n      \"description\": \"The current composition status of the contract.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the contract was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the contract was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/json-schema/schema-contract.json
tags:
- Federation
- GraphQL
- Management
- Schema Registry
title: WunderGraph Cosmo Schema Contract
---
