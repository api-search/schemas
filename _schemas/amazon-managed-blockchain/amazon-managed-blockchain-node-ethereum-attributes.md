---
description: Attributes of an Ethereum node.
layout: schema
name: NodeEthereumAttributes
properties_list:
- description: ''
  name: HttpEndpoint
  type: object
- description: ''
  name: WebSocketEndpoint
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-node-ethereum-attributes-schema.json
slug: amazon-managed-blockchain-node-ethereum-attributes
source_filename: amazon-managed-blockchain-node-ethereum-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-node-ethereum-attributes-schema.json\",\n  \"title\": \"NodeEthereumAttributes\",\n  \"description\": \"Attributes of an Ethereum node.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HttpEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The endpoint on which the Ethereum node listens to run Ethereum API methods over HTTP connections from a client. Use this endpoint in client code for smart contracts when using an HTTP connection. Connections to this endpoint are authenticated using <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/signature-version-4.html\\\">Signature Version 4</a>.\"\n        }\n      ]\n    },\n    \"WebSocketEndpoint\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The endpoint on which the Ethereum node listens to run Ethereum JSON-RPC methods over WebSocket connections from a client. Use this endpoint in client code for smart contracts when using a WebSocket connection. Connections to this endpoint are authenticated using <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/signature-version-4.html\\\">Signature Version 4</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-node-ethereum-attributes-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: NodeEthereumAttributes
---
