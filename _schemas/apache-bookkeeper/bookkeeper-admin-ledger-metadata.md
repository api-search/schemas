---
description: Metadata for a single BookKeeper ledger.
layout: schema
name: LedgerMetadata
properties_list:
- description: Unique identifier of the ledger.
  name: ledgerId
  type: integer
- description: Number of bookies in the ensemble.
  name: ensembleSize
  type: integer
- description: Number of bookies to write to per entry.
  name: writeQuorumSize
  type: integer
- description: Number of acks required before an entry is considered written.
  name: ackQuorumSize
  type: integer
- description: State of the ledger (OPEN or CLOSED).
  name: state
  type: string
- description: Total byte length of the ledger.
  name: length
  type: integer
- description: ID of the last entry in the ledger.
  name: lastEntryId
  type: integer
provider_name: Apache BookKeeper
provider_slug: apache-bookkeeper
schema_file: json-schema/bookkeeper-admin-ledger-metadata-schema.json
slug: bookkeeper-admin-ledger-metadata
tags:
- Apache
- Distributed Systems
- Log Storage
- Open Source
- Storage
- Streaming
title: LedgerMetadata
---
