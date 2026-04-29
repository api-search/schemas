---
description: BookKeeper cluster-wide status and bookie count information.
layout: schema
name: ClusterInfo
properties_list:
- description: Whether an auditor has been elected.
  name: auditorElected
  type: boolean
- description: Socket address of the elected auditor.
  name: auditorId
  type: string
- description: Whether any ledgers in the cluster are under-replicated.
  name: clusterUnderReplicated
  type: boolean
- description: Whether ledger replication is enabled.
  name: ledgerReplicationEnabled
  type: boolean
- description: Total number of bookies in the cluster.
  name: totalBookiesCount
  type: integer
- description: Number of bookies available for writes.
  name: writableBookiesCount
  type: integer
- description: Number of read-only bookies.
  name: readonlyBookiesCount
  type: integer
- description: Number of unavailable bookies.
  name: unavailableBookiesCount
  type: integer
provider_name: Apache BookKeeper
provider_slug: apache-bookkeeper
schema_file: json-schema/bookkeeper-admin-cluster-info-schema.json
slug: bookkeeper-admin-cluster-info
source_filename: bookkeeper-admin-cluster-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-bookkeeper/refs/heads/main/json-schema/bookkeeper-admin-cluster-info-schema.json\",\n  \"title\": \"ClusterInfo\",\n  \"description\": \"BookKeeper cluster-wide status and bookie count information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"auditorElected\": { \"type\": \"boolean\", \"description\": \"Whether an auditor has been elected.\", \"example\": true },\n    \"auditorId\": { \"type\": \"string\", \"description\": \"Socket address of the elected auditor.\", \"example\": \"bookie1.example.com:3181\" },\n    \"clusterUnderReplicated\": { \"type\": \"boolean\", \"description\": \"Whether any ledgers in the cluster are under-replicated.\", \"example\": false },\n    \"ledgerReplicationEnabled\": { \"type\": \"boolean\", \"description\": \"Whether ledger replication is enabled.\", \"example\": true },\n    \"totalBookiesCount\"\
  : { \"type\": \"integer\", \"description\": \"Total number of bookies in the cluster.\", \"example\": 3 },\n    \"writableBookiesCount\": { \"type\": \"integer\", \"description\": \"Number of bookies available for writes.\", \"example\": 3 },\n    \"readonlyBookiesCount\": { \"type\": \"integer\", \"description\": \"Number of read-only bookies.\", \"example\": 0 },\n    \"unavailableBookiesCount\": { \"type\": \"integer\", \"description\": \"Number of unavailable bookies.\", \"example\": 0 }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-bookkeeper/refs/heads/main/json-schema/bookkeeper-admin-cluster-info-schema.json
tags:
- Apache
- Distributed Systems
- Log Storage
- Open Source
- Storage
- Streaming
title: ClusterInfo
---
