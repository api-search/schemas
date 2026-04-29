---
description: Configuration properties of a node.
layout: schema
name: NodeConfiguration
properties_list:
- description: ''
  name: InstanceType
  type: object
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: LogPublishingConfiguration
  type: object
- description: ''
  name: StateDB
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-node-configuration-schema.json
slug: amazon-managed-blockchain-node-configuration
source_filename: amazon-managed-blockchain-node-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-node-configuration-schema.json\",\n  \"title\": \"NodeConfiguration\",\n  \"description\": \"Configuration properties of a node.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceTypeString\"\n        },\n        {\n          \"description\": \"The Amazon Managed Blockchain instance type for the node.\"\n        }\n      ]\n    },\n    \"AvailabilityZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailabilityZoneString\"\n        },\n        {\n          \"description\": \"The Availability Zone in which the node exists. Required for Ethereum nodes. \"\n        }\n      ]\n    },\n    \"LogPublishingConfiguration\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeLogPublishingConfiguration\"\n        },\n        {\n          \"description\": \"Configuration properties for logging events associated with a peer node on a Hyperledger Fabric network on Managed Blockchain. \"\n        }\n      ]\n    },\n    \"StateDB\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateDBType\"\n        },\n        {\n          \"description\": \"<p>The state database that the node uses. Values are <code>LevelDB</code> or <code>CouchDB</code>. When using an Amazon Managed Blockchain network with Hyperledger Fabric version 1.4 or later, the default is <code>CouchDB</code>.</p> <p>Applies only to Hyperledger Fabric.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InstanceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-node-configuration-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: NodeConfiguration
---
