---
description: <p>An action to invite a specific Amazon Web Services account to create a member and join the network. The <code>InviteAction</code> is carried out when a <code>Proposal</code> is <code>APPROVED</code>.</p> <p>Applies only to Hyperledger Fabric.</p>
layout: schema
name: InviteAction
properties_list:
- description: ''
  name: Principal
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-invite-action-schema.json
slug: amazon-managed-blockchain-invite-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-invite-action-schema.json\",\n  \"title\": \"InviteAction\",\n  \"description\": \"<p>An action to invite a specific Amazon Web Services account to create a member and join the network. The <code>InviteAction</code> is carried out when a <code>Proposal</code> is <code>APPROVED</code>.</p> <p>Applies only to Hyperledger Fabric.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Principal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrincipalString\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID to invite.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Principal\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-invite-action-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: InviteAction
---
