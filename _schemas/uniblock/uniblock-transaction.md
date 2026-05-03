---
description: Schema representing a blockchain transaction with detailed execution information as returned by the Uniblock Unified API.
layout: schema
name: Uniblock Transaction
properties_list:
- description: The unique hash identifier of the transaction.
  name: transactionHash
  type: string
- description: The sender address.
  name: from
  type: string
- description: The recipient address.
  name: to
  type: string
- description: The value transferred in the native token's smallest unit.
  name: value
  type: string
- description: The block number containing the transaction.
  name: blockNumber
  type: integer
- description: The timestamp of the block containing the transaction.
  name: blockTimestamp
  type: string
- description: The execution status of the transaction.
  name: status
  type: string
- description: The amount of gas consumed by the transaction.
  name: gasUsed
  type: string
- description: The gas price at which the transaction was executed.
  name: gasPrice
  type: string
- description: The sender's transaction nonce.
  name: nonce
  type: integer
- description: The input data of the transaction in hexadecimal format.
  name: input
  type: string
- description: Event logs emitted during the transaction execution.
  name: logs
  type: array
provider_name: Uniblock
provider_slug: uniblock
schema_file: json-schema/uniblock-transaction-schema.json
slug: uniblock-transaction
source_filename: uniblock-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://uniblock.dev/schemas/uniblock/transaction.json\",\n  \"title\": \"Uniblock Transaction\",\n  \"description\": \"Schema representing a blockchain transaction with detailed execution information as returned by the Uniblock Unified API.\",\n  \"type\": \"object\",\n  \"required\": [\"transactionHash\"],\n  \"properties\": {\n    \"transactionHash\": {\n      \"type\": \"string\",\n      \"description\": \"The unique hash identifier of the transaction.\",\n      \"pattern\": \"^0x[a-fA-F0-9]{64}$\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"The sender address.\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"description\": \"The recipient address.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value transferred in the native token's smallest unit.\"\n    },\n    \"blockNumber\": {\n      \"type\": \"\
  integer\",\n      \"description\": \"The block number containing the transaction.\",\n      \"minimum\": 0\n    },\n    \"blockTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp of the block containing the transaction.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The execution status of the transaction.\",\n      \"enum\": [\"success\", \"failed\"]\n    },\n    \"gasUsed\": {\n      \"type\": \"string\",\n      \"description\": \"The amount of gas consumed by the transaction.\"\n    },\n    \"gasPrice\": {\n      \"type\": \"string\",\n      \"description\": \"The gas price at which the transaction was executed.\"\n    },\n    \"nonce\": {\n      \"type\": \"integer\",\n      \"description\": \"The sender's transaction nonce.\",\n      \"minimum\": 0\n    },\n    \"input\": {\n      \"type\": \"string\",\n      \"description\": \"The input data of the transaction in hexadecimal format.\"\
  \n    },\n    \"logs\": {\n      \"type\": \"array\",\n      \"description\": \"Event logs emitted during the transaction execution.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TransactionLog\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"TransactionLog\": {\n      \"type\": \"object\",\n      \"description\": \"An event log emitted by a smart contract during transaction execution.\",\n      \"properties\": {\n        \"logIndex\": {\n          \"type\": \"integer\",\n          \"description\": \"The position of the log entry in the block.\",\n          \"minimum\": 0\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"The smart contract address that emitted the event.\"\n        },\n        \"topics\": {\n          \"type\": \"array\",\n          \"description\": \"Indexed event topics used for filtering and identification.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"minItems\": 1,\n   \
  \       \"maxItems\": 4\n        },\n        \"data\": {\n          \"type\": \"string\",\n          \"description\": \"Non-indexed event data in hexadecimal format.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/uniblock/refs/heads/main/json-schema/uniblock-transaction-schema.json
tags:
- Blockchain
- Web3
title: Uniblock Transaction
---
