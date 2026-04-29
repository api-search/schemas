---
description: drep_votes schema from Blockfrost API
layout: schema
name: drep_votes
properties_list: []
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-drep-votes-schema.json
slug: blockfrost-drep-votes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-drep-votes-schema.json\",\n  \"title\": \"drep_votes\",\n  \"description\": \"drep_votes schema from Blockfrost API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"tx_hash\": {\n        \"type\": \"string\",\n        \"description\": \"Hash of the vote transaction.\"\n      },\n      \"cert_index\": {\n        \"type\": \"integer\",\n        \"description\": \"Index of the certificate within the vote transaction.\"\n      },\n      \"proposal_id\": {\n        \"type\": \"string\",\n        \"description\": \"Governance Action Identifier (CIP-0129) of the proposal being voted on.\"\n      },\n      \"proposal_tx_hash\": {\n        \"type\": \"string\",\n        \"description\": \"Hash of the proposal transaction.\"\n      },\n      \"proposal_cert_index\"\
  : {\n        \"type\": \"integer\",\n        \"description\": \"Index of the certificate within the proposal transaction.\"\n      },\n      \"vote\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"yes\",\n          \"no\",\n          \"abstain\"\n        ],\n        \"description\": \"The Vote. Can be one of yes, no, abstain.\"\n      }\n    },\n    \"required\": [\n      \"tx_hash\",\n      \"cert_index\",\n      \"proposal_id\",\n      \"proposal_tx_hash\",\n      \"proposal_cert_index\",\n      \"vote\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-drep-votes-schema.json
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: drep_votes
---
