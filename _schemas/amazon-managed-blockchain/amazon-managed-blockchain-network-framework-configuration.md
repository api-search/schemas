---
description: Configuration properties relevant to the network for the blockchain framework that the network uses.
layout: schema
name: NetworkFrameworkConfiguration
properties_list:
- description: ''
  name: Fabric
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-network-framework-configuration-schema.json
slug: amazon-managed-blockchain-network-framework-configuration
source_filename: amazon-managed-blockchain-network-framework-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-network-framework-configuration-schema.json\",\n  \"title\": \"NetworkFrameworkConfiguration\",\n  \"description\": \" Configuration properties relevant to the network for the blockchain framework that the network uses. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Fabric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkFabricConfiguration\"\n        },\n        {\n          \"description\": \" Hyperledger Fabric configuration properties for a Managed Blockchain network that uses Hyperledger Fabric. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-network-framework-configuration-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: NetworkFrameworkConfiguration
---
