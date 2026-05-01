---
description: VoteOnProposalInput schema from Amazon Managed Blockchain API
layout: schema
name: VoteOnProposalInput
properties_list:
- description: ''
  name: VoterMemberId
  type: object
- description: ''
  name: Vote
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-vote-on-proposal-input-schema.json
slug: amazon-managed-blockchain-vote-on-proposal-input
source_filename: amazon-managed-blockchain-vote-on-proposal-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-vote-on-proposal-input-schema.json\",\n  \"title\": \"VoteOnProposalInput\",\n  \"description\": \"VoteOnProposalInput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VoterMemberId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the member casting the vote. \"\n        }\n      ]\n    },\n    \"Vote\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VoteValue\"\n        },\n        {\n          \"description\": \" The value of the vote. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VoterMemberId\",\n    \"Vote\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-vote-on-proposal-input-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: VoteOnProposalInput
---
