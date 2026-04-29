---
description: CreateMemberInput schema from Amazon Managed Blockchain API
layout: schema
name: CreateMemberInput
properties_list:
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: InvitationId
  type: object
- description: ''
  name: MemberConfiguration
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-create-member-input-schema.json
slug: amazon-managed-blockchain-create-member-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-create-member-input-schema.json\",\n  \"title\": \"CreateMemberInput\",\n  \"description\": \"CreateMemberInput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestTokenString\"\n        },\n        {\n          \"description\": \"A unique, case-sensitive identifier that you provide to ensure the idempotency of the operation. An idempotent operation completes no more than one time. This identifier is required only if you make a service request directly using an HTTP client. It is generated automatically if you use an Amazon Web Services SDK or the CLI.\"\n        }\n      ]\n    },\n    \"InvitationId\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the invitation that is sent to the member to join the network.\"\n        }\n      ]\n    },\n    \"MemberConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberConfiguration\"\n        },\n        {\n          \"description\": \"Member configuration parameters.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ClientRequestToken\",\n    \"InvitationId\",\n    \"MemberConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-create-member-input-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: CreateMemberInput
---
