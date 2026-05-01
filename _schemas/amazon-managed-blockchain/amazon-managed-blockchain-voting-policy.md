---
description: <p> The voting rules for the network to decide if a proposal is accepted </p> <p>Applies only to Hyperledger Fabric.</p>
layout: schema
name: VotingPolicy
properties_list:
- description: ''
  name: ApprovalThresholdPolicy
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-voting-policy-schema.json
slug: amazon-managed-blockchain-voting-policy
source_filename: amazon-managed-blockchain-voting-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-voting-policy-schema.json\",\n  \"title\": \"VotingPolicy\",\n  \"description\": \"<p> The voting rules for the network to decide if a proposal is accepted </p> <p>Applies only to Hyperledger Fabric.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApprovalThresholdPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApprovalThresholdPolicy\"\n        },\n        {\n          \"description\": \"Defines the rules for the network for voting on proposals, such as the percentage of <code>YES</code> votes required for the proposal to be approved and the duration of the proposal. The policy applies to all proposals and is specified when the network is created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-voting-policy-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: VotingPolicy
---
