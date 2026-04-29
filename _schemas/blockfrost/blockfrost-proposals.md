---
description: proposals schema from Blockfrost API
layout: schema
name: proposals
properties_list: []
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-proposals-schema.json
slug: blockfrost-proposals
source_filename: blockfrost-proposals-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-proposals-schema.json\",\n  \"title\": \"proposals\",\n  \"description\": \"proposals schema from Blockfrost API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"id\": {\n        \"type\": \"string\",\n        \"description\": \"Governance Action Identifier (CIP-0129)\"\n      },\n      \"tx_hash\": {\n        \"type\": \"string\",\n        \"description\": \"Hash of the proposal transaction.\"\n      },\n      \"cert_index\": {\n        \"type\": \"integer\",\n        \"description\": \"Index of the certificate within the proposal transaction.\"\n      },\n      \"governance_type\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"hard_fork_initiation\",\n          \"new_committee\",\n          \"new_constitution\",\n       \
  \   \"info_action\",\n          \"no_confidence\",\n          \"parameter_change\",\n          \"treasury_withdrawals\"\n        ],\n        \"description\": \"Type of proposal.\"\n      }\n    },\n    \"required\": [\n      \"id\",\n      \"tx_hash\",\n      \"cert_index\",\n      \"governance_type\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-proposals-schema.json
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: proposals
---
