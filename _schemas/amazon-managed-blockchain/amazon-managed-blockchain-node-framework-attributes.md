---
description: Attributes relevant to a node on a Managed Blockchain network for the blockchain framework that the network uses.
layout: schema
name: NodeFrameworkAttributes
properties_list:
- description: ''
  name: Fabric
  type: object
- description: ''
  name: Ethereum
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-node-framework-attributes-schema.json
slug: amazon-managed-blockchain-node-framework-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-node-framework-attributes-schema.json\",\n  \"title\": \"NodeFrameworkAttributes\",\n  \"description\": \"Attributes relevant to a node on a Managed Blockchain network for the blockchain framework that the network uses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Fabric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeFabricAttributes\"\n        },\n        {\n          \"description\": \"Attributes of Hyperledger Fabric for a peer node on a Managed Blockchain network that uses Hyperledger Fabric.\"\n        }\n      ]\n    },\n    \"Ethereum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeEthereumAttributes\"\n        },\n        {\n          \"description\": \"Attributes of Ethereum\
  \ for a node on a Managed Blockchain network that uses Ethereum. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-node-framework-attributes-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: NodeFrameworkAttributes
---
