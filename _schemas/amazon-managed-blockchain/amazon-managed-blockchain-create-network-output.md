---
description: CreateNetworkOutput schema from Amazon Managed Blockchain API
layout: schema
name: CreateNetworkOutput
properties_list:
- description: ''
  name: NetworkId
  type: object
- description: ''
  name: MemberId
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-create-network-output-schema.json
slug: amazon-managed-blockchain-create-network-output
source_filename: amazon-managed-blockchain-create-network-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-create-network-output-schema.json\",\n  \"title\": \"CreateNetworkOutput\",\n  \"description\": \"CreateNetworkOutput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NetworkId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier for the network.\"\n        }\n      ]\n    },\n    \"MemberId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier for the first member within the network.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-create-network-output-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: CreateNetworkOutput
---
