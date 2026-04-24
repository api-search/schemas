---
description: block_content schema from Blockfrost API
layout: schema
name: block_content
properties_list:
- description: Block creation time in UNIX time
  name: time
  type: integer
- description: Block number
  name: height
  type: integer
- description: Hash of the block
  name: hash
  type: string
- description: Slot number
  name: slot
  type: integer
- description: Epoch number
  name: epoch
  type: integer
- description: Slot within the epoch
  name: epoch_slot
  type: integer
- description: Bech32 ID of the slot leader or specific block description in case there is no slot leader
  name: slot_leader
  type: string
- description: Block size in Bytes
  name: size
  type: integer
- description: Number of transactions in the block
  name: tx_count
  type: integer
- description: Total output within the block in Lovelaces
  name: output
  type: string
- description: Total fees within the block in Lovelaces
  name: fees
  type: string
- description: VRF key of the block
  name: block_vrf
  type: string
- description: The hash of the operational certificate of the block producer
  name: op_cert
  type: string
- description: The value of the counter used to produce the operational certificate
  name: op_cert_counter
  type: string
- description: Hash of the previous block
  name: previous_block
  type: string
- description: Hash of the next block
  name: next_block
  type: string
- description: Number of block confirmations
  name: confirmations
  type: integer
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-block-content-schema.json
slug: blockfrost-block-content
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: block_content
---
