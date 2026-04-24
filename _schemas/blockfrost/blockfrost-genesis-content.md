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
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: genesis_content
---
