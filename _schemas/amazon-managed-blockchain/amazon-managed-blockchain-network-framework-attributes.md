---
description: Attributes relevant to the network for the blockchain framework that the network uses.
layout: schema
name: NetworkFrameworkAttributes
properties_list:
- description: ''
  name: Fabric
  type: object
- description: ''
  name: Ethereum
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-network-framework-attributes-schema.json
slug: amazon-managed-blockchain-network-framework-attributes
source_filename: amazon-managed-blockchain-network-framework-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-network-framework-attributes-schema.json\",\n  \"title\": \"NetworkFrameworkAttributes\",\n  \"description\": \"Attributes relevant to the network for the blockchain framework that the network uses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Fabric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkFabricAttributes\"\n        },\n        {\n          \"description\": \"Attributes of Hyperledger Fabric for a Managed Blockchain network that uses Hyperledger Fabric.\"\n        }\n      ]\n    },\n    \"Ethereum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkEthereumAttributes\"\n        },\n        {\n          \"description\": \"Attributes of an Ethereum network for Managed Blockchain\
  \ resources participating in an Ethereum network. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-network-framework-attributes-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: NetworkFrameworkAttributes
---
