---
description: ListInvitationsOutput schema from Amazon Managed Blockchain API
layout: schema
name: ListInvitationsOutput
properties_list:
- description: ''
  name: Invitations
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-list-invitations-output-schema.json
slug: amazon-managed-blockchain-list-invitations-output
source_filename: amazon-managed-blockchain-list-invitations-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-list-invitations-output-schema.json\",\n  \"title\": \"ListInvitationsOutput\",\n  \"description\": \"ListInvitationsOutput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Invitations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InvitationList\"\n        },\n        {\n          \"description\": \"The invitations for the network.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The pagination token that indicates the next set of results to retrieve.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-list-invitations-output-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: ListInvitationsOutput
---
