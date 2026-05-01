---
description: CreateProposalInput schema from Amazon Managed Blockchain API
layout: schema
name: CreateProposalInput
properties_list:
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: MemberId
  type: object
- description: ''
  name: Actions
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-create-proposal-input-schema.json
slug: amazon-managed-blockchain-create-proposal-input
source_filename: amazon-managed-blockchain-create-proposal-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-create-proposal-input-schema.json\",\n  \"title\": \"CreateProposalInput\",\n  \"description\": \"CreateProposalInput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestTokenString\"\n        },\n        {\n          \"description\": \"A unique, case-sensitive identifier that you provide to ensure the idempotency of the operation. An idempotent operation completes no more than one time. This identifier is required only if you make a service request directly using an HTTP client. It is generated automatically if you use an Amazon Web Services SDK or the CLI.\"\n        }\n      ]\n    },\n    \"MemberId\": {\n \
  \     \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the member that is creating the proposal. This identifier is especially useful for identifying the member making the proposal when multiple members exist in a single Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"Actions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProposalActions\"\n        },\n        {\n          \"description\": \"The type of actions proposed, such as inviting a member or removing a member. The types of <code>Actions</code> in a proposal are mutually exclusive. For example, a proposal with <code>Invitations</code> actions cannot also contain <code>Removals</code> actions.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n \
  \         \"description\": \"A description for the proposal that is visible to voting members, for example, \\\"Proposal to add Example Corp. as member.\\\"\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputTagMap\"\n        },\n        {\n          \"description\": \"<p>Tags to assign to the proposal.</p> <p> Each tag consists of a key and an optional value. You can specify multiple key-value pairs in a single request with an overall maximum of 50 tags allowed per resource.</p> <p>For more information about tags, see <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/ethereum-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Ethereum Developer Guide</i>, or <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/hyperledger-fabric-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Hyperledger Fabric Developer\
  \ Guide</i>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ClientRequestToken\",\n    \"MemberId\",\n    \"Actions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-create-proposal-input-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: CreateProposalInput
---
