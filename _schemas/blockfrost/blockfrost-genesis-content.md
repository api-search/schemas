---
description: genesis_content schema from Blockfrost API
layout: schema
name: genesis_content
properties_list:
- description: The proportion of slots in which blocks should be issued
  name: active_slots_coefficient
  type: number
- description: Determines the quorum needed for votes on the protocol parameter updates
  name: update_quorum
  type: integer
- description: The total number of lovelace in the system
  name: max_lovelace_supply
  type: string
- description: Network identifier
  name: network_magic
  type: integer
- description: Number of slots in an epoch
  name: epoch_length
  type: integer
- description: Time of slot 0 in UNIX time
  name: system_start
  type: integer
- description: Number of slots in an KES period
  name: slots_per_kes_period
  type: integer
- description: Duration of one slot in seconds
  name: slot_length
  type: integer
- description: The maximum number of time a KES key can be evolved before a pool operator must create a new operational certificate
  name: max_kes_evolutions
  type: integer
- description: Security parameter k
  name: security_param
  type: integer
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-genesis-content-schema.json
slug: blockfrost-genesis-content
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-genesis-content-schema.json\",\n  \"title\": \"genesis_content\",\n  \"description\": \"genesis_content schema from Blockfrost API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"active_slots_coefficient\": {\n      \"type\": \"number\",\n      \"example\": 0.05,\n      \"description\": \"The proportion of slots in which blocks should be issued\"\n    },\n    \"update_quorum\": {\n      \"type\": \"integer\",\n      \"example\": 5,\n      \"description\": \"Determines the quorum needed for votes on the protocol parameter updates\"\n    },\n    \"max_lovelace_supply\": {\n      \"type\": \"string\",\n      \"example\": \"45000000000000000\",\n      \"description\": \"The total number of lovelace in the system\"\n    },\n    \"network_magic\": {\n      \"type\": \"integer\",\n      \"example\"\
  : 764824073,\n      \"description\": \"Network identifier\"\n    },\n    \"epoch_length\": {\n      \"type\": \"integer\",\n      \"example\": 432000,\n      \"description\": \"Number of slots in an epoch\"\n    },\n    \"system_start\": {\n      \"type\": \"integer\",\n      \"example\": 1506203091,\n      \"description\": \"Time of slot 0 in UNIX time\"\n    },\n    \"slots_per_kes_period\": {\n      \"type\": \"integer\",\n      \"example\": 129600,\n      \"description\": \"Number of slots in an KES period\"\n    },\n    \"slot_length\": {\n      \"type\": \"integer\",\n      \"example\": 1,\n      \"description\": \"Duration of one slot in seconds\"\n    },\n    \"max_kes_evolutions\": {\n      \"type\": \"integer\",\n      \"example\": 62,\n      \"description\": \"The maximum number of time a KES key can be evolved before a pool operator must create a new operational certificate\"\n    },\n    \"security_param\": {\n      \"type\": \"integer\",\n      \"example\": 2160,\n      \"\
  description\": \"Security parameter k\"\n    }\n  },\n  \"required\": [\n    \"active_slots_coefficient\",\n    \"update_quorum\",\n    \"max_lovelace_supply\",\n    \"network_magic\",\n    \"epoch_length\",\n    \"system_start\",\n    \"slots_per_kes_period\",\n    \"slot_length\",\n    \"max_kes_evolutions\",\n    \"security_param\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-genesis-content-schema.json
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: genesis_content
---
