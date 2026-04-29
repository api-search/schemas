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
source_filename: bookkeeper-admin-ledger-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-bookkeeper/refs/heads/main/json-schema/bookkeeper-admin-ledger-metadata-schema.json\",\n  \"title\": \"LedgerMetadata\",\n  \"description\": \"Metadata for a single BookKeeper ledger.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ledgerId\": { \"type\": \"integer\", \"format\": \"int64\", \"description\": \"Unique identifier of the ledger.\", \"example\": 12345 },\n    \"ensembleSize\": { \"type\": \"integer\", \"description\": \"Number of bookies in the ensemble.\", \"example\": 3 },\n    \"writeQuorumSize\": { \"type\": \"integer\", \"description\": \"Number of bookies to write to per entry.\", \"example\": 2 },\n    \"ackQuorumSize\": { \"type\": \"integer\", \"description\": \"Number of acks required before an entry is considered written.\", \"example\": 2 },\n    \"state\": { \"type\": \"string\", \"description\": \"State of\
  \ the ledger (OPEN or CLOSED).\", \"enum\": [\"OPEN\", \"CLOSED\"], \"example\": \"CLOSED\" },\n    \"length\": { \"type\": \"integer\", \"format\": \"int64\", \"description\": \"Total byte length of the ledger.\", \"example\": 1048576 },\n    \"lastEntryId\": { \"type\": \"integer\", \"format\": \"int64\", \"description\": \"ID of the last entry in the ledger.\", \"example\": 1024 }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-bookkeeper/refs/heads/main/json-schema/bookkeeper-admin-ledger-metadata-schema.json
tags:
- Apache
- Distributed Systems
- Log Storage
- Open Source
- Storage
- Streaming
title: LedgerMetadata
---
