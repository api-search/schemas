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
source_filename: blockfrost-block-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-block-content-schema.json\",\n  \"title\": \"block_content\",\n  \"description\": \"block_content schema from Blockfrost API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"time\": {\n      \"type\": \"integer\",\n      \"example\": 1641338934,\n      \"description\": \"Block creation time in UNIX time\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"example\": 15243593,\n      \"description\": \"Block number\"\n    },\n    \"hash\": {\n      \"type\": \"string\",\n      \"example\": \"4ea1ba291e8eef538635a53e59fddba7810d1679631cc3aed7c8e6c4091a516a\",\n      \"description\": \"Hash of the block\"\n    },\n    \"slot\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"example\": 412162133,\n      \"description\": \"Slot number\"\
  \n    },\n    \"epoch\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"example\": 425,\n      \"description\": \"Epoch number\"\n    },\n    \"epoch_slot\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"example\": 12,\n      \"description\": \"Slot within the epoch\"\n    },\n    \"slot_leader\": {\n      \"type\": \"string\",\n      \"example\": \"pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2qnikdy\",\n      \"description\": \"Bech32 ID of the slot leader or specific block description in case there is no slot leader\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"example\": 3,\n      \"description\": \"Block size in Bytes\"\n    },\n    \"tx_count\": {\n      \"type\": \"integer\",\n      \"example\": 1,\n      \"description\": \"Number of transactions in the block\"\n    },\n    \"output\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"128314491794\",\n      \"description\": \"Total output\
  \ within the block in Lovelaces\"\n    },\n    \"fees\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"592661\",\n      \"description\": \"Total fees within the block in Lovelaces\"\n    },\n    \"block_vrf\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"vrf_vk1wf2k6lhujezqcfe00l6zetxpnmh9n6mwhpmhm0dvfh3fxgmdnrfqkms8ty\",\n      \"description\": \"VRF key of the block\",\n      \"minLength\": 65,\n      \"maxLength\": 65\n    },\n    \"op_cert\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"da905277534faf75dae41732650568af545134ee08a3c0392dbefc8096ae177c\",\n      \"description\": \"The hash of the operational certificate of the block producer\"\n    },\n    \"op_cert_counter\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"18\",\n      \"description\": \"The value of the counter used to produce the operational certificate\"\n    },\n    \"previous_block\"\
  : {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"43ebccb3ac72c7cebd0d9b755a4b08412c9f5dcb81b8a0ad1e3c197d29d47b05\",\n      \"description\": \"Hash of the previous block\"\n    },\n    \"next_block\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"8367f026cf4b03e116ff8ee5daf149b55ba5a6ec6dec04803b8dc317721d15fa\",\n      \"description\": \"Hash of the next block\"\n    },\n    \"confirmations\": {\n      \"type\": \"integer\",\n      \"example\": 4698,\n      \"description\": \"Number of block confirmations\"\n    }\n  },\n  \"required\": [\n    \"time\",\n    \"height\",\n    \"hash\",\n    \"slot\",\n    \"epoch\",\n    \"epoch_slot\",\n    \"slot_leader\",\n    \"size\",\n    \"tx_count\",\n    \"output\",\n    \"fees\",\n    \"block_vrf\",\n    \"op_cert\",\n    \"op_cert_counter\",\n    \"previous_block\",\n    \"next_block\",\n    \"confirmations\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-block-content-schema.json
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: block_content
---
