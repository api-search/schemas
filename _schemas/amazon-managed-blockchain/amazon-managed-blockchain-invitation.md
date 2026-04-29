---
description: <p>An invitation to an Amazon Web Services account to create a member and join the network.</p> <p>Applies only to Hyperledger Fabric.</p>
layout: schema
name: Invitation
properties_list:
- description: ''
  name: InvitationId
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: ExpirationDate
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: NetworkSummary
  type: object
- description: ''
  name: Arn
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-invitation-schema.json
slug: amazon-managed-blockchain-invitation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-invitation-schema.json\",\n  \"title\": \"Invitation\",\n  \"description\": \"<p>An invitation to an Amazon Web Services account to create a member and join the network.</p> <p>Applies only to Hyperledger Fabric.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InvitationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier for the invitation.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time that the invitation was created.\"\n        }\n      ]\n    },\n    \"ExpirationDate\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time that the invitation expires. This is the <code>CreationDate</code> plus the <code>ProposalDurationInHours</code> that is specified in the <code>ProposalThresholdPolicy</code>. After this date and time, the invitee can no longer create a member and join the network using this <code>InvitationId</code>.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InvitationStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the invitation:</p> <ul> <li> <p> <code>PENDING</code> - The invitee hasn't created a member to join the network, and the invitation hasn't yet expired.</p> </li> <li> <p> <code>ACCEPTING</code> - The invitee has begun creating a member, and creation hasn't yet completed.</p> </li> <li> <p> <code>ACCEPTED</code> - The invitee\
  \ created a member and joined the network using the <code>InvitationID</code>.</p> </li> <li> <p> <code>REJECTED</code> - The invitee rejected the invitation.</p> </li> <li> <p> <code>EXPIRED</code> - The invitee neither created a member nor rejected the invitation before the <code>ExpirationDate</code>.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"NetworkSummary\": {\n      \"$ref\": \"#/components/schemas/NetworkSummary\"\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the invitation. For more information about ARNs and their format, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in the <i>Amazon Web Services General Reference</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-invitation-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: Invitation
---
