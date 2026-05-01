---
description: Attributes of Ethereum for a network.
layout: schema
name: NetworkEthereumAttributes
properties_list:
- description: ''
  name: ChainId
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-network-ethereum-attributes-schema.json
slug: amazon-managed-blockchain-network-ethereum-attributes
source_filename: amazon-managed-blockchain-network-ethereum-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-network-ethereum-attributes-schema.json\",\n  \"title\": \"NetworkEthereumAttributes\",\n  \"description\": \"Attributes of Ethereum for a network. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChainId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The Ethereum <code>CHAIN_ID</code> associated with the Ethereum network. Chain IDs are as follows:</p> <ul> <li> <p>mainnet = <code>1</code> </p> </li> <li> <p>goerli = <code>5</code> </p> </li> <li> <p>rinkeby = <code>4</code> </p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-network-ethereum-attributes-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: NetworkEthereumAttributes
---
