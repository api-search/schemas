---
description: Hyperledger Fabric configuration properties for the network.
layout: schema
name: NetworkFabricConfiguration
properties_list:
- description: ''
  name: Edition
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-network-fabric-configuration-schema.json
slug: amazon-managed-blockchain-network-fabric-configuration
source_filename: amazon-managed-blockchain-network-fabric-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-network-fabric-configuration-schema.json\",\n  \"title\": \"NetworkFabricConfiguration\",\n  \"description\": \"Hyperledger Fabric configuration properties for the network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Edition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Edition\"\n        },\n        {\n          \"description\": \"The edition of Amazon Managed Blockchain that the network uses. For more information, see <a href=\\\"http://aws.amazon.com/managed-blockchain/pricing/\\\">Amazon Managed Blockchain Pricing</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Edition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-network-fabric-configuration-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: NetworkFabricConfiguration
---
