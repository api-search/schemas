---
description: dreps schema from Blockfrost API
layout: schema
name: dreps
properties_list: []
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-dreps-schema.json
slug: blockfrost-dreps
source_filename: blockfrost-dreps-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-dreps-schema.json\",\n  \"title\": \"dreps\",\n  \"description\": \"dreps schema from Blockfrost API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"drep_id\": {\n        \"type\": \"string\",\n        \"description\": \"The Bech32 encoded DRep address\"\n      },\n      \"hex\": {\n        \"type\": \"string\",\n        \"description\": \"The raw bytes of the DRep\"\n      }\n    },\n    \"required\": [\n      \"drep_id\",\n      \"hex\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-dreps-schema.json
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: dreps
---
