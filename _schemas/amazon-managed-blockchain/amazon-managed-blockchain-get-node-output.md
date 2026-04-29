---
description: GetNodeOutput schema from Amazon Managed Blockchain API
layout: schema
name: GetNodeOutput
properties_list:
- description: ''
  name: Node
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-get-node-output-schema.json
slug: amazon-managed-blockchain-get-node-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-get-node-output-schema.json\",\n  \"title\": \"GetNodeOutput\",\n  \"description\": \"GetNodeOutput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Node\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Node\"\n        },\n        {\n          \"description\": \"Properties of the node configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-get-node-output-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: GetNodeOutput
---
