---
description: UpdateNodeInput schema from Amazon Managed Blockchain API
layout: schema
name: UpdateNodeInput
properties_list:
- description: ''
  name: MemberId
  type: object
- description: ''
  name: LogPublishingConfiguration
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-update-node-input-schema.json
slug: amazon-managed-blockchain-update-node-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-update-node-input-schema.json\",\n  \"title\": \"UpdateNodeInput\",\n  \"description\": \"UpdateNodeInput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MemberId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"<p>The unique identifier of the member that owns the node.</p> <p>Applies only to Hyperledger Fabric.</p>\"\n        }\n      ]\n    },\n    \"LogPublishingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeLogPublishingConfiguration\"\n        },\n        {\n          \"description\": \"Configuration properties for publishing to Amazon CloudWatch Logs.\"\n     \
  \   }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-update-node-input-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: UpdateNodeInput
---
