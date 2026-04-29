---
description: drep_updates schema from Blockfrost API
layout: schema
name: drep_updates
properties_list: []
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-drep-updates-schema.json
slug: blockfrost-drep-updates
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-drep-updates-schema.json\",\n  \"title\": \"drep_updates\",\n  \"description\": \"drep_updates schema from Blockfrost API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"tx_hash\": {\n        \"type\": \"string\",\n        \"description\": \"Transaction ID\"\n      },\n      \"cert_index\": {\n        \"type\": \"integer\",\n        \"description\": \"Index of the certificate within the update transaction.\"\n      },\n      \"action\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"registered\",\n          \"deregistered\",\n          \"updated\"\n        ],\n        \"description\": \"Action in the certificate\"\n      }\n    },\n    \"required\": [\n      \"tx_hash\",\n      \"cert_index\",\n      \"action\"\n    ]\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-drep-updates-schema.json
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: drep_updates
---
