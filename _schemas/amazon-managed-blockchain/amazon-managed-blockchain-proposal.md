---
description: <p>Properties of a proposal on a Managed Blockchain network.</p> <p>Applies only to Hyperledger Fabric.</p>
layout: schema
name: Proposal
properties_list:
- description: ''
  name: ProposalId
  type: object
- description: ''
  name: NetworkId
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Actions
  type: object
- description: ''
  name: ProposedByMemberId
  type: object
- description: ''
  name: ProposedByMemberName
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: ExpirationDate
  type: object
- description: ''
  name: YesVoteCount
  type: object
- description: ''
  name: NoVoteCount
  type: object
- description: ''
  name: OutstandingVoteCount
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Arn
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-proposal-schema.json
slug: amazon-managed-blockchain-proposal
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-proposal-schema.json\",\n  \"title\": \"Proposal\",\n  \"description\": \"<p>Properties of a proposal on a Managed Blockchain network.</p> <p>Applies only to Hyperledger Fabric.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProposalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the proposal.\"\n        }\n      ]\n    },\n    \"NetworkId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the network for which the proposal is made.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"The description of the proposal.\"\n        }\n      ]\n    },\n    \"Actions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProposalActions\"\n        },\n        {\n          \"description\": \"The actions to perform on the network if the proposal is <code>APPROVED</code>.\"\n        }\n      ]\n    },\n    \"ProposedByMemberId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the member that created the proposal.\"\n        }\n      ]\n    },\n    \"ProposedByMemberName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkMemberNameString\"\n        },\n        {\n          \"description\": \"The name of the member that created the proposal.\"\n        }\n      ]\n\
  \    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProposalStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the proposal. Values are as follows:</p> <ul> <li> <p> <code>IN_PROGRESS</code> - The proposal is active and open for member voting.</p> </li> <li> <p> <code>APPROVED</code> - The proposal was approved with sufficient <code>YES</code> votes among members according to the <code>VotingPolicy</code> specified for the <code>Network</code>. The specified proposal actions are carried out.</p> </li> <li> <p> <code>REJECTED</code> - The proposal was rejected with insufficient <code>YES</code> votes among members according to the <code>VotingPolicy</code> specified for the <code>Network</code>. The specified <code>ProposalActions</code> aren't carried out.</p> </li> <li> <p> <code>EXPIRED</code> - Members didn't cast the number of votes required to determine the proposal outcome before the proposal expired. The\
  \ specified <code>ProposalActions</code> aren't carried out.</p> </li> <li> <p> <code>ACTION_FAILED</code> - One or more of the specified <code>ProposalActions</code> in a proposal that was approved couldn't be completed because of an error. The <code>ACTION_FAILED</code> status occurs even if only one ProposalAction fails and other actions are successful.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The date and time that the proposal was created. \"\n        }\n      ]\n    },\n    \"ExpirationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The date and time that the proposal expires. This is the <code>CreationDate</code> plus the <code>ProposalDurationInHours</code> that is specified in the <code>ProposalThresholdPolicy</code>.\
  \ After this date and time, if members haven't cast enough votes to determine the outcome according to the voting policy, the proposal is <code>EXPIRED</code> and <code>Actions</code> aren't carried out. \"\n        }\n      ]\n    },\n    \"YesVoteCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VoteCount\"\n        },\n        {\n          \"description\": \" The current total of <code>YES</code> votes cast on the proposal by members. \"\n        }\n      ]\n    },\n    \"NoVoteCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VoteCount\"\n        },\n        {\n          \"description\": \" The current total of <code>NO</code> votes cast on the proposal by members. \"\n        }\n      ]\n    },\n    \"OutstandingVoteCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VoteCount\"\n        },\n        {\n          \"description\": \" The number of votes remaining to be cast on the\
  \ proposal by members. In other words, the number of members minus the sum of <code>YES</code> votes and <code>NO</code> votes. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputTagMap\"\n        },\n        {\n          \"description\": \"<p>Tags assigned to the proposal. Each tag consists of a key and optional value.</p> <p>For more information about tags, see <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/ethereum-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Ethereum Developer Guide</i>, or <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/hyperledger-fabric-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Hyperledger Fabric Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnString\"\n      \
  \  },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the proposal. For more information about ARNs and their format, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in the <i>Amazon Web Services General Reference</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-proposal-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: Proposal
---
