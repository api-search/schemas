---
description: Configuration properties for logging events associated with a peer node owned by a member in a Managed Blockchain network.
layout: schema
name: NodeFabricLogPublishingConfiguration
properties_list:
- description: ''
  name: ChaincodeLogs
  type: object
- description: ''
  name: PeerLogs
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-node-fabric-log-publishing-configuration-schema.json
slug: amazon-managed-blockchain-node-fabric-log-publishing-configuration
source_filename: amazon-managed-blockchain-node-fabric-log-publishing-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-node-fabric-log-publishing-configuration-schema.json\",\n  \"title\": \"NodeFabricLogPublishingConfiguration\",\n  \"description\": \"Configuration properties for logging events associated with a peer node owned by a member in a Managed Blockchain network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChaincodeLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogConfigurations\"\n        },\n        {\n          \"description\": \"Configuration properties for logging events associated with chaincode execution on a peer node. Chaincode logs contain the results of instantiating, invoking, and querying the chaincode. A peer can run multiple instances of chaincode. When enabled, a log stream is created for all chaincodes, with\
  \ an individual log stream for each chaincode.\"\n        }\n      ]\n    },\n    \"PeerLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogConfigurations\"\n        },\n        {\n          \"description\": \"Configuration properties for a peer node log. Peer node logs contain messages generated when your client submits transaction proposals to peer nodes, requests to join channels, enrolls an admin peer, and lists the chaincode instances on a peer node. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-node-fabric-log-publishing-configuration-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: NodeFabricLogPublishingConfiguration
---
