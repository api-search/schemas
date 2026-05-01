---
description: GetProposalOutput schema from Amazon Managed Blockchain API
layout: schema
name: GetProposalOutput
properties_list:
- description: ''
  name: Proposal
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-get-proposal-output-schema.json
slug: amazon-managed-blockchain-get-proposal-output
source_filename: amazon-managed-blockchain-get-proposal-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-get-proposal-output-schema.json\",\n  \"title\": \"GetProposalOutput\",\n  \"description\": \"GetProposalOutput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Proposal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Proposal\"\n        },\n        {\n          \"description\": \"Information about a proposal.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-get-proposal-output-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: GetProposalOutput
---
