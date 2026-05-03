---
description: Schema representing a non-fungible token with metadata, collection information, and transfer data as returned by the Uniblock Unified API.
layout: schema
name: Uniblock NFT
properties_list:
- description: The smart contract address of the NFT collection.
  name: contractAddress
  type: string
- description: The unique token ID within the collection.
  name: tokenId
  type: string
- description: The name of the NFT.
  name: name
  type: string
- description: A description of the NFT.
  name: description
  type: string
- description: The token standard type.
  name: tokenType
  type: string
- description: URL to the NFT image.
  name: imageUrl
  type: string
- description: URL to the NFT animation or media file.
  name: animationUrl
  type: string
- description: The name of the parent collection.
  name: collectionName
  type: string
- description: List of trait attributes for the NFT.
  name: attributes
  type: array
provider_name: Uniblock
provider_slug: uniblock
schema_file: json-schema/uniblock-nft-schema.json
slug: uniblock-nft
source_filename: uniblock-nft-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://uniblock.dev/schemas/uniblock/nft.json\",\n  \"title\": \"Uniblock NFT\",\n  \"description\": \"Schema representing a non-fungible token with metadata, collection information, and transfer data as returned by the Uniblock Unified API.\",\n  \"type\": \"object\",\n  \"required\": [\"contractAddress\", \"tokenId\"],\n  \"properties\": {\n    \"contractAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The smart contract address of the NFT collection.\"\n    },\n    \"tokenId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token ID within the collection.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the NFT.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the NFT.\"\n    },\n    \"tokenType\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The token standard type.\",\n      \"enum\": [\"ERC-721\", \"ERC-1155\"]\n    },\n    \"imageUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the NFT image.\"\n    },\n    \"animationUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the NFT animation or media file.\"\n    },\n    \"collectionName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the parent collection.\"\n    },\n    \"attributes\": {\n      \"type\": \"array\",\n      \"description\": \"List of trait attributes for the NFT.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/NftAttribute\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"NftAttribute\": {\n      \"type\": \"object\",\n      \"description\": \"A trait attribute associated with an NFT.\",\n      \"required\": [\"traitType\", \"value\"],\n      \"properties\": {\n        \"traitType\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The name of the trait category.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The value of the trait.\"\n        }\n      }\n    },\n    \"NftCollection\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about an NFT collection.\",\n      \"required\": [\"contractAddress\"],\n      \"properties\": {\n        \"contractAddress\": {\n          \"type\": \"string\",\n          \"description\": \"The smart contract address of the collection.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the collection.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the collection.\"\n        },\n        \"symbol\": {\n          \"type\": \"string\",\n          \"description\": \"The symbol of the collection.\"\n        },\n        \"totalSupply\": {\n          \"type\": \"integer\",\n          \"\
  description\": \"The total number of NFTs in the collection.\",\n          \"minimum\": 0\n        },\n        \"imageUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the collection image.\"\n        },\n        \"floorPrice\": {\n          \"type\": \"number\",\n          \"description\": \"The current floor price of the collection.\",\n          \"minimum\": 0\n        },\n        \"chain\": {\n          \"type\": \"string\",\n          \"description\": \"The blockchain network the collection exists on.\"\n        }\n      }\n    },\n    \"NftTransfer\": {\n      \"type\": \"object\",\n      \"description\": \"An NFT transfer event between two addresses.\",\n      \"required\": [\"transactionHash\", \"from\", \"to\", \"contractAddress\", \"tokenId\"],\n      \"properties\": {\n        \"transactionHash\": {\n          \"type\": \"string\",\n          \"description\": \"The hash of the transaction containing this transfer.\"\
  ,\n          \"pattern\": \"^0x[a-fA-F0-9]{64}$\"\n        },\n        \"from\": {\n          \"type\": \"string\",\n          \"description\": \"The sender address.\"\n        },\n        \"to\": {\n          \"type\": \"string\",\n          \"description\": \"The recipient address.\"\n        },\n        \"contractAddress\": {\n          \"type\": \"string\",\n          \"description\": \"The smart contract address of the NFT collection.\"\n        },\n        \"tokenId\": {\n          \"type\": \"string\",\n          \"description\": \"The token ID of the transferred NFT.\"\n        },\n        \"tokenType\": {\n          \"type\": \"string\",\n          \"description\": \"The token standard type.\",\n          \"enum\": [\"ERC-721\", \"ERC-1155\"]\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of tokens transferred (relevant for ERC-1155).\",\n          \"minimum\": 1\n        },\n        \"blockNumber\": {\n        \
  \  \"type\": \"integer\",\n          \"description\": \"The block number in which the transfer occurred.\",\n          \"minimum\": 0\n        },\n        \"blockTimestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp of the block in which the transfer occurred.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/uniblock/refs/heads/main/json-schema/uniblock-nft-schema.json
tags:
- Blockchain
- Web3
title: Uniblock NFT
---
