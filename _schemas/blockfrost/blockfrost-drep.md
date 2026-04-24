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
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: drep
---
