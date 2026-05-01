---
description: Attributes of Hyperledger Fabric for a network.
layout: schema
name: NetworkFabricAttributes
properties_list:
- description: ''
  name: OrderingServiceEndpoint
  type: object
- description: ''
  name: Edition
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-network-fabric-attributes-schema.json
slug: amazon-managed-blockchain-network-fabric-attributes
source_filename: amazon-managed-blockchain-network-fabric-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-network-fabric-attributes-schema.json\",\n  \"title\": \"NetworkFabricAttributes\",\n  \"description\": \"Attributes of Hyperledger Fabric for a network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrderingServiceEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The endpoint of the ordering service for the network.\"\n        }\n      ]\n    },\n    \"Edition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Edition\"\n        },\n        {\n          \"description\": \"The edition of Amazon Managed Blockchain that Hyperledger Fabric uses. For more information, see <a href=\\\"http://aws.amazon.com/managed-blockchain/pricing/\\\
  \">Amazon Managed Blockchain Pricing</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-network-fabric-attributes-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: NetworkFabricAttributes
---
