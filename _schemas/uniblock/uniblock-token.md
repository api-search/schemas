---
description: Schema representing a fungible token with metadata, balance, and transfer information as returned by the Uniblock Unified API.
layout: schema
name: Uniblock Token
properties_list:
- description: The smart contract address of the token on the blockchain.
  name: contractAddress
  type: string
- description: The blockchain network identifier (e.g., ethereum, polygon, solana).
  name: chain
  type: string
- description: The display name of the token.
  name: name
  type: string
- description: The ticker symbol of the token.
  name: symbol
  type: string
- description: The number of decimal places the token uses.
  name: decimals
  type: integer
- description: URL to the token logo image.
  name: logo
  type: string
- description: The total supply of the token in its smallest unit.
  name: totalSupply
  type: string
provider_name: Uniblock
provider_slug: uniblock
schema_file: json-schema/uniblock-token-schema.json
slug: uniblock-token
source_filename: uniblock-token-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://uniblock.dev/schemas/uniblock/token.json\",\n  \"title\": \"Uniblock Token\",\n  \"description\": \"Schema representing a fungible token with metadata, balance, and transfer information as returned by the Uniblock Unified API.\",\n  \"type\": \"object\",\n  \"required\": [\"contractAddress\", \"chain\"],\n  \"properties\": {\n    \"contractAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The smart contract address of the token on the blockchain.\"\n    },\n    \"chain\": {\n      \"type\": \"string\",\n      \"description\": \"The blockchain network identifier (e.g., ethereum, polygon, solana).\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the token.\"\n    },\n    \"symbol\": {\n      \"type\": \"string\",\n      \"description\": \"The ticker symbol of the token.\",\n      \"maxLength\": 20\n    },\n    \"decimals\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"The number of decimal places the token uses.\",\n      \"minimum\": 0,\n      \"maximum\": 18\n    },\n    \"logo\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the token logo image.\"\n    },\n    \"totalSupply\": {\n      \"type\": \"string\",\n      \"description\": \"The total supply of the token in its smallest unit.\",\n      \"pattern\": \"^[0-9]+$\"\n    }\n  },\n  \"$defs\": {\n    \"TokenBalance\": {\n      \"type\": \"object\",\n      \"description\": \"Balance of a specific token held by a wallet address.\",\n      \"required\": [\"contractAddress\", \"balance\"],\n      \"properties\": {\n        \"contractAddress\": {\n          \"type\": \"string\",\n          \"description\": \"The smart contract address of the token.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the token.\"\n        },\n   \
  \     \"symbol\": {\n          \"type\": \"string\",\n          \"description\": \"The ticker symbol of the token.\"\n        },\n        \"decimals\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of decimal places the token uses.\",\n          \"minimum\": 0\n        },\n        \"balance\": {\n          \"type\": \"string\",\n          \"description\": \"The token balance in its smallest unit.\",\n          \"pattern\": \"^[0-9]+$\"\n        },\n        \"balanceFormatted\": {\n          \"type\": \"string\",\n          \"description\": \"The token balance formatted with proper decimal places.\"\n        }\n      }\n    },\n    \"TokenTransfer\": {\n      \"type\": \"object\",\n      \"description\": \"A token transfer event between two addresses on the blockchain.\",\n      \"required\": [\"transactionHash\", \"from\", \"to\", \"value\"],\n      \"properties\": {\n        \"transactionHash\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The hash of the transaction containing this transfer.\",\n          \"pattern\": \"^0x[a-fA-F0-9]{64}$\"\n        },\n        \"from\": {\n          \"type\": \"string\",\n          \"description\": \"The sender address.\"\n        },\n        \"to\": {\n          \"type\": \"string\",\n          \"description\": \"The recipient address.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The amount transferred in the token's smallest unit.\"\n        },\n        \"contractAddress\": {\n          \"type\": \"string\",\n          \"description\": \"The smart contract address of the transferred token.\"\n        },\n        \"tokenName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the transferred token.\"\n        },\n        \"tokenSymbol\": {\n          \"type\": \"string\",\n          \"description\": \"The symbol of the transferred token.\"\n        },\n        \"blockNumber\": {\n          \"type\"\
  : \"integer\",\n          \"description\": \"The block number in which the transfer occurred.\",\n          \"minimum\": 0\n        },\n        \"blockTimestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp of the block in which the transfer occurred.\"\n        }\n      }\n    },\n    \"TokenAllowance\": {\n      \"type\": \"object\",\n      \"description\": \"A token spending allowance granted to a spender contract.\",\n      \"required\": [\"contractAddress\", \"spender\", \"allowance\"],\n      \"properties\": {\n        \"contractAddress\": {\n          \"type\": \"string\",\n          \"description\": \"The smart contract address of the token.\"\n        },\n        \"spender\": {\n          \"type\": \"string\",\n          \"description\": \"The address of the approved spender.\"\n        },\n        \"allowance\": {\n          \"type\": \"string\",\n          \"description\": \"The approved allowance amount\
  \ in the token's smallest unit.\"\n        },\n        \"tokenName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the token.\"\n        },\n        \"tokenSymbol\": {\n          \"type\": \"string\",\n          \"description\": \"The symbol of the token.\"\n        }\n      }\n    },\n    \"TokenPrice\": {\n      \"type\": \"object\",\n      \"description\": \"Price data for a token from aggregated market sources.\",\n      \"properties\": {\n        \"usdPrice\": {\n          \"type\": \"number\",\n          \"description\": \"The current price of the token in USD.\",\n          \"minimum\": 0\n        },\n        \"chain\": {\n          \"type\": \"string\",\n          \"description\": \"The blockchain network.\"\n        },\n        \"contractAddress\": {\n          \"type\": \"string\",\n          \"description\": \"The contract address of the token.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/uniblock/refs/heads/main/json-schema/uniblock-token-schema.json
tags:
- Blockchain
- Web3
title: Uniblock Token
---
