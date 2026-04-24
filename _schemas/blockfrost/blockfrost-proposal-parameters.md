---
description: proposal_parameters schema from Blockfrost API
layout: schema
name: proposal_parameters
properties_list:
- description: Governance Action Identifier (CIP-0129)
  name: id
  type: string
- description: Off-chain metadata of a proposal with a specific transaction hash
  name: tx_hash
  type: string
- description: Off-chain metadata of a proposal with a specific transaction cert_index
  name: cert_index
  type: integer
- description: ''
  name: parameters
  type: object
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-proposal-parameters-schema.json
slug: blockfrost-proposal-parameters
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: proposal_parameters
---
