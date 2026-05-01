---
description: <p> Properties of an individual vote that a member cast for a proposal. </p> <p>Applies only to Hyperledger Fabric.</p>
layout: schema
name: VoteSummary
properties_list:
- description: ''
  name: Vote
  type: object
- description: ''
  name: MemberName
  type: object
- description: ''
  name: MemberId
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-vote-summary-schema.json
slug: amazon-managed-blockchain-vote-summary
source_filename: amazon-managed-blockchain-vote-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-vote-summary-schema.json\",\n  \"title\": \"VoteSummary\",\n  \"description\": \"<p> Properties of an individual vote that a member cast for a proposal. </p> <p>Applies only to Hyperledger Fabric.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Vote\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VoteValue\"\n        },\n        {\n          \"description\": \" The vote value, either <code>YES</code> or <code>NO</code>. \"\n        }\n      ]\n    },\n    \"MemberName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkMemberNameString\"\n        },\n        {\n          \"description\": \" The name of the member that cast the vote. \"\n        }\n      ]\n    },\n    \"MemberId\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \" The unique identifier of the member that cast the vote. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-vote-summary-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: VoteSummary
---
