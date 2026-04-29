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
source_filename: blockfrost-proposal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-proposal-schema.json\",\n  \"title\": \"proposal\",\n  \"description\": \"proposal schema from Blockfrost API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Governance Action Identifier (CIP-0129)\"\n    },\n    \"tx_hash\": {\n      \"type\": \"string\",\n      \"description\": \"Hash of the proposal transaction.\"\n    },\n    \"cert_index\": {\n      \"type\": \"integer\",\n      \"description\": \"Index of the certificate within the proposal transaction.\"\n    },\n    \"governance_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"hard_fork_initiation\",\n        \"new_committee\",\n        \"new_constitution\",\n        \"info_action\",\n        \"no_confidence\",\n        \"parameter_change\",\n     \
  \   \"treasury_withdrawals\"\n      ],\n      \"description\": \"Type of proposal.\"\n    },\n    \"governance_description\": {\n      \"additionalProperties\": true,\n      \"type\": \"object\",\n      \"nullable\": true,\n      \"description\": \"An object describing the content of this GovActionProposal in a readable way.\"\n    },\n    \"deposit\": {\n      \"type\": \"string\",\n      \"description\": \"The deposit amount paid for this proposal.\"\n    },\n    \"return_address\": {\n      \"type\": \"string\",\n      \"description\": \"Bech32 stake address of the reward address to receive the deposit when it is repaid.\"\n    },\n    \"ratified_epoch\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"The epoch at which the proposal was ratified. Null if the proposal has not been ratified.\"\n    },\n    \"enacted_epoch\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"The epoch at which the proposal was enacted.\
  \ Null if the proposal has not been enacted.\"\n    },\n    \"dropped_epoch\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"The epoch at which the proposal was dropped. A proposal is dropped if it expires or if any of its dependencies expire.\"\n    },\n    \"expired_epoch\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"The epoch at which the proposal expired. Null if the proposal has not expired.\"\n    },\n    \"expiration\": {\n      \"type\": \"integer\",\n      \"description\": \"The epoch at which this governance action will expire.\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"tx_hash\",\n    \"cert_index\",\n    \"governance_type\",\n    \"deposit\",\n    \"return_address\",\n    \"governance_description\",\n    \"ratified_epoch\",\n    \"enacted_epoch\",\n    \"dropped_epoch\",\n    \"expired_epoch\",\n    \"expiration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-proposal-schema.json
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: proposal
---
