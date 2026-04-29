---
description: CreateProposalOutput schema from Amazon Managed Blockchain API
layout: schema
name: CreateProposalOutput
properties_list:
- description: ''
  name: ProposalId
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-create-proposal-output-schema.json
slug: amazon-managed-blockchain-create-proposal-output
source_filename: amazon-managed-blockchain-create-proposal-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-create-proposal-output-schema.json\",\n  \"title\": \"CreateProposalOutput\",\n  \"description\": \"CreateProposalOutput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProposalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the proposal.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-create-proposal-output-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: CreateProposalOutput
---
