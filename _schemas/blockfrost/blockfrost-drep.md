---
description: drep schema from Blockfrost API
layout: schema
name: drep
properties_list:
- description: Bech32 encoded DRep address
  name: drep_id
  type: string
- description: The raw bytes of the DRep
  name: hex
  type: string
- description: The total amount of voting power this DRep is delegated.
  name: amount
  type: string
- description: Registration state of the DRep
  name: active
  type: boolean
- description: Epoch of the most recent registration
  name: active_epoch
  type: integer
- description: Flag which shows if this DRep credentials are a script hash
  name: has_script
  type: boolean
- description: Registration state of the DRep. Set to `true` if the DRep has been deregistered; otherwise, `false`.
  name: retired
  type: boolean
- description: Whether the DRep has been inactive for a consecutive number of epochs (determined by a epoch parameter `drep_activity`)
  name: expired
  type: boolean
- description: Epoch of the most recent action - registration, update, deregistration or voting
  name: last_active_epoch
  type: integer
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-drep-schema.json
slug: blockfrost-drep
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-drep-schema.json\",\n  \"title\": \"drep\",\n  \"description\": \"drep schema from Blockfrost API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"drep_id\": {\n      \"type\": \"string\",\n      \"description\": \"Bech32 encoded DRep address\"\n    },\n    \"hex\": {\n      \"type\": \"string\",\n      \"description\": \"The raw bytes of the DRep\"\n    },\n    \"amount\": {\n      \"type\": \"string\",\n      \"description\": \"The total amount of voting power this DRep is delegated.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Registration state of the DRep\",\n      \"deprecated\": true\n    },\n    \"active_epoch\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Epoch of the most recent registration\",\n   \
  \   \"deprecated\": true\n    },\n    \"has_script\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag which shows if this DRep credentials are a script hash\"\n    },\n    \"retired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Registration state of the DRep. Set to `true` if the DRep has been deregistered; otherwise, `false`.\"\n    },\n    \"expired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DRep has been inactive for a consecutive number of epochs (determined by a epoch parameter `drep_activity`)\"\n    },\n    \"last_active_epoch\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Epoch of the most recent action - registration, update, deregistration or voting\"\n    }\n  },\n  \"required\": [\n    \"drep_id\",\n    \"hex\",\n    \"amount\",\n    \"active\",\n    \"active_epoch\",\n    \"has_script\",\n    \"retired\",\n    \"expired\",\n    \"last_active_epoch\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-drep-schema.json
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: drep
---
