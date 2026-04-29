---
description: proposal_withdrawals schema from Blockfrost API
layout: schema
name: proposal_withdrawals
properties_list: []
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-proposal-withdrawals-schema.json
slug: blockfrost-proposal-withdrawals
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-proposal-withdrawals-schema.json\",\n  \"title\": \"proposal_withdrawals\",\n  \"description\": \"proposal_withdrawals schema from Blockfrost API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"stake_address\": {\n        \"type\": \"string\",\n        \"example\": \"stake1ux3g2c9dx2nhhehyrezyxpkstartcqmu9hk63qgfkccw5rqttygt7\",\n        \"description\": \"Bech32 stake address\"\n      },\n      \"amount\": {\n        \"type\": \"string\",\n        \"description\": \"Withdrawal amount in Lovelaces\"\n      }\n    },\n    \"required\": [\n      \"stake_address\",\n      \"amount\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-proposal-withdrawals-schema.json
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: proposal_withdrawals
---
