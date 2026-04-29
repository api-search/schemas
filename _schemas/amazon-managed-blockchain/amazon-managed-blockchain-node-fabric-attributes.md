---
description: Attributes of Hyperledger Fabric for a peer node on a Hyperledger Fabric network on Managed Blockchain.
layout: schema
name: NodeFabricAttributes
properties_list:
- description: ''
  name: PeerEndpoint
  type: object
- description: ''
  name: PeerEventEndpoint
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-node-fabric-attributes-schema.json
slug: amazon-managed-blockchain-node-fabric-attributes
source_filename: amazon-managed-blockchain-node-fabric-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-node-fabric-attributes-schema.json\",\n  \"title\": \"NodeFabricAttributes\",\n  \"description\": \"Attributes of Hyperledger Fabric for a peer node on a Hyperledger Fabric network on Managed Blockchain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PeerEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The endpoint that identifies the peer node for all services except peer channel-based event services.\"\n        }\n      ]\n    },\n    \"PeerEventEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The endpoint that identifies the peer node for peer channel-based\
  \ event services.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-node-fabric-attributes-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: NodeFabricAttributes
---
