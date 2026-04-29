---
description: drep_metadata schema from Blockfrost API
layout: schema
name: drep_metadata
properties_list:
- description: Bech32 encoded addresses
  name: drep_id
  type: string
- description: The raw bytes of the DRep
  name: hex
  type: string
- description: URL to the drep metadata
  name: url
  type: string
- description: Hash of the metadata file
  name: hash
  type: string
- description: Content of the JSON metadata (validated CIP-119)
  name: json_metadata
  type: object
- description: Content of the metadata (raw)
  name: bytes
  type: string
- description: Present when metadata could not be fetched or validated.
  name: error
  type: object
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-drep-metadata-schema.json
slug: blockfrost-drep-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-drep-metadata-schema.json\",\n  \"title\": \"drep_metadata\",\n  \"description\": \"drep_metadata schema from Blockfrost API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"drep_id\": {\n      \"type\": \"string\",\n      \"description\": \"Bech32 encoded addresses\"\n    },\n    \"hex\": {\n      \"type\": \"string\",\n      \"description\": \"The raw bytes of the DRep\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://stakenuts.com/drep.json\",\n      \"description\": \"URL to the drep metadata\"\n    },\n    \"hash\": {\n      \"type\": \"string\",\n      \"example\": \"69c0c68cb57f4a5b4a87bad896fc274678e7aea98e200fa14a1cb40c0cab1d8c\\\"\",\n      \"description\": \"Hash of the metadata file\"\n    },\n    \"json_metadata\": {\n      \"anyOf\": [\n   \
  \     {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        },\n        {\n          \"type\": \"array\",\n          \"items\": {}\n        },\n        {\n          \"type\": \"integer\"\n        },\n        {\n          \"type\": \"number\"\n        },\n        {\n          \"type\": \"boolean\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"description\": \"Content of the JSON metadata (validated CIP-119)\"\n    },\n    \"bytes\": {\n      \"type\": \"string\",\n      \"description\": \"Content of the metadata (raw)\",\n      \"nullable\": true\n    },\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"Present when metadata could not be fetched or validated.\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Stable machine-readable error code.\",\n          \"enum\": [\n          \
  \  \"HASH_MISMATCH\",\n            \"CONNECTION_ERROR\",\n            \"HTTP_RESPONSE_ERROR\",\n            \"DECODE_ERROR\",\n            \"SIZE_EXCEEDED\",\n            \"UNKNOWN_ERROR\"\n          ]\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of the error.\"\n        }\n      },\n      \"required\": [\n        \"code\",\n        \"message\"\n      ]\n    }\n  },\n  \"required\": [\n    \"drep_id\",\n    \"hex\",\n    \"url\",\n    \"hash\",\n    \"json_metadata\",\n    \"bytes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-drep-metadata-schema.json
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: drep_metadata
---
