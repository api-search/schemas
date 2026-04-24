---
description: proposal schema from Blockfrost API
layout: schema
name: proposal
properties_list:
- description: Governance Action Identifier (CIP-0129)
  name: id
  type: string
- description: Hash of the proposal transaction.
  name: tx_hash
  type: string
- description: Index of the certificate within the proposal transaction.
  name: cert_index
  type: integer
- description: Type of proposal.
  name: governance_type
  type: string
- description: An object describing the content of this GovActionProposal in a readable way.
  name: governance_description
  type: object
- description: The deposit amount paid for this proposal.
  name: deposit
  type: string
- description: Bech32 stake address of the reward address to receive the deposit when it is repaid.
  name: return_address
  type: string
- description: The epoch at which the proposal was ratified. Null if the proposal has not been ratified.
  name: ratified_epoch
  type: integer
- description: The epoch at which the proposal was enacted. Null if the proposal has not been enacted.
  name: enacted_epoch
  type: integer
- description: The epoch at which the proposal was dropped. A proposal is dropped if it expires or if any of its dependencies expire.
  name: dropped_epoch
  type: integer
- description: The epoch at which the proposal expired. Null if the proposal has not expired.
  name: expired_epoch
  type: integer
- description: The epoch at which this governance action will expire.
  name: expiration
  type: integer
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-proposal-schema.json
slug: blockfrost-proposal
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: proposal
---
