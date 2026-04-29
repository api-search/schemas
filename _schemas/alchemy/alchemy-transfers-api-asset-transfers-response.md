---
description: JSON-RPC response for getAssetTransfers requests.
layout: schema
name: Asset Transfers Response
properties_list:
- description: Matches the request ID.
  name: id
  type: integer
- description: JSON-RPC version.
  name: jsonrpc
  type: string
- description: Result payload containing the list of asset transfers.
  name: result
  type: object
provider_name: Alchemy
provider_slug: alchemy
schema_file: json-schema/alchemy-transfers-api-asset-transfers-response-schema.json
slug: alchemy-transfers-api-asset-transfers-response
source_filename: alchemy-transfers-api-asset-transfers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-transfers-api-asset-transfers-response-schema.json\",\n  \"title\": \"Asset Transfers Response\",\n  \"description\": \"JSON-RPC response for getAssetTransfers requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Matches the request ID.\",\n      \"example\": 1\n    },\n    \"jsonrpc\": {\n      \"type\": \"string\",\n      \"description\": \"JSON-RPC version.\",\n      \"example\": \"2.0\"\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"title\": \"Asset Transfers Result\",\n      \"description\": \"Result payload containing the list of asset transfers.\",\n      \"properties\": {\n        \"transfers\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"\
  title\": \"Asset Transfer\",\n            \"description\": \"Represents a single asset transfer event on the blockchain.\",\n            \"properties\": {\n              \"blockNum\": {\n                \"type\": \"string\",\n                \"description\": \"Block number of the transfer in hexadecimal.\",\n                \"example\": \"0xfda53c\"\n              },\n              \"hash\": {\n                \"type\": \"string\",\n                \"description\": \"Transaction hash of the transfer.\",\n                \"example\": \"0xabc123def456abc123def456abc123def456\"\n              },\n              \"from\": {\n                \"type\": \"string\",\n                \"description\": \"Sender wallet address.\",\n                \"example\": \"0x0000000000000000000000000000000000000000\"\n              },\n              \"to\": {\n                \"type\": \"string\",\n                \"description\": \"Recipient wallet address.\",\n                \"example\": \"0xd8da6bf26964af9d7eed9e03e53415d37aa96045\"\
  \n              },\n              \"value\": {\n                \"type\": \"number\",\n                \"description\": \"Transfer value in native units.\",\n                \"example\": 1.0\n              },\n              \"asset\": {\n                \"type\": \"string\",\n                \"description\": \"Asset symbol (e.g., ETH, USDC, or NFT collection name).\",\n                \"example\": \"ETH\"\n              },\n              \"category\": {\n                \"type\": \"string\",\n                \"description\": \"Transfer category (external, internal, erc20, erc721, erc1155).\",\n                \"enum\": [\n                  \"external\",\n                  \"internal\",\n                  \"erc20\",\n                  \"erc721\",\n                  \"erc1155\"\n                ],\n                \"example\": \"external\"\n              },\n              \"metadata\": {\n                \"type\": \"object\",\n                \"title\": \"Transfer Metadata\",\n         \
  \       \"description\": \"Additional metadata for an asset transfer.\",\n                \"properties\": {\n                  \"blockTimestamp\": {\n                    \"type\": \"string\",\n                    \"format\": \"date-time\",\n                    \"description\": \"ISO 8601 timestamp of the block.\",\n                    \"example\": \"2026-04-19T10:00:00Z\"\n                  }\n                }\n              }\n            }\n          },\n          \"description\": \"List of asset transfer events matching the query.\"\n        },\n        \"pageKey\": {\n          \"type\": \"string\",\n          \"description\": \"Pagination key for retrieving the next page of results.\",\n          \"example\": \"abc123nextpage\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-transfers-api-asset-transfers-response-schema.json
tags:
- Blockchain
- Cryptocurrency
- Web3
- Account Abstraction
- Ethereum
title: Asset Transfers Response
---
