---
description: <p> The actions to carry out if a proposal is <code>APPROVED</code>. </p> <p>Applies only to Hyperledger Fabric.</p>
layout: schema
name: ProposalActions
properties_list:
- description: ''
  name: Invitations
  type: object
- description: ''
  name: Removals
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-proposal-actions-schema.json
slug: amazon-managed-blockchain-proposal-actions
source_filename: amazon-managed-blockchain-proposal-actions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-proposal-actions-schema.json\",\n  \"title\": \"ProposalActions\",\n  \"description\": \"<p> The actions to carry out if a proposal is <code>APPROVED</code>. </p> <p>Applies only to Hyperledger Fabric.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Invitations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InviteActionList\"\n        },\n        {\n          \"description\": \" The actions to perform for an <code>APPROVED</code> proposal to invite an Amazon Web Services account to create a member and join the network. \"\n        }\n      ]\n    },\n    \"Removals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemoveActionList\"\n        },\n        {\n          \"description\": \" The actions\
  \ to perform for an <code>APPROVED</code> proposal to remove a member from the network, which deletes the member and all associated member resources from the network. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-proposal-actions-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: ProposalActions
---
