---
description: drep_delegators schema from Blockfrost API
layout: schema
name: drep_delegators
properties_list: []
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-drep-delegators-schema.json
slug: blockfrost-drep-delegators
source_filename: blockfrost-drep-delegators-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-drep-delegators-schema.json\",\n  \"title\": \"drep_delegators\",\n  \"description\": \"drep_delegators schema from Blockfrost API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"address\": {\n        \"type\": \"string\",\n        \"description\": \"Bech32 encoded stake addresses\"\n      },\n      \"amount\": {\n        \"type\": \"string\",\n        \"description\": \"Currently delegated amount\"\n      }\n    },\n    \"required\": [\n      \"address\",\n      \"amount\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-drep-delegators-schema.json
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: drep_delegators
---
