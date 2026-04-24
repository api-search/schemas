---
description: drep_metadata schema from Blockfrost API
layout: schema
name: drep_metadata
properties_list:
- description: Bech32 encoded addresses
  name: drep_id
  type: string
- description: The raw bytes of the DRep
  name: hex
  type: string
- description: URL to the drep metadata
  name: url
  type: string
- description: Hash of the metadata file
  name: hash
  type: string
- description: Content of the JSON metadata (validated CIP-119)
  name: json_metadata
  type: object
- description: Content of the metadata (raw)
  name: bytes
  type: string
- description: Present when metadata could not be fetched or validated.
  name: error
  type: object
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-drep-metadata-schema.json
slug: blockfrost-drep-metadata
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: drep_metadata
---
