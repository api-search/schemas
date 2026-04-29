---
description: <p>A policy type that defines the voting rules for the network. The rules decide if a proposal is approved. Approval may be based on criteria such as the percentage of <code>YES</code> votes and the duration of the proposal. The policy applies to all proposals and is specified when the network is created.</p> <p>Applies only to Hyperledger Fabric.</p>
layout: schema
name: ApprovalThresholdPolicy
properties_list:
- description: ''
  name: ThresholdPercentage
  type: object
- description: ''
  name: ProposalDurationInHours
  type: object
- description: ''
  name: ThresholdComparator
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-approval-threshold-policy-schema.json
slug: amazon-managed-blockchain-approval-threshold-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-approval-threshold-policy-schema.json\",\n  \"title\": \"ApprovalThresholdPolicy\",\n  \"description\": \"<p>A policy type that defines the voting rules for the network. The rules decide if a proposal is approved. Approval may be based on criteria such as the percentage of <code>YES</code> votes and the duration of the proposal. The policy applies to all proposals and is specified when the network is created.</p> <p>Applies only to Hyperledger Fabric.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ThresholdPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThresholdPercentageInt\"\n        },\n        {\n          \"description\": \"The percentage of votes among all members that must be <code>YES</code> for a proposal\
  \ to be approved. For example, a <code>ThresholdPercentage</code> value of <code>50</code> indicates 50%. The <code>ThresholdComparator</code> determines the precise comparison. If a <code>ThresholdPercentage</code> value of <code>50</code> is specified on a network with 10 members, along with a <code>ThresholdComparator</code> value of <code>GREATER_THAN</code>, this indicates that 6 <code>YES</code> votes are required for the proposal to be approved.\"\n        }\n      ]\n    },\n    \"ProposalDurationInHours\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProposalDurationInt\"\n        },\n        {\n          \"description\": \"The duration from the time that a proposal is created until it expires. If members cast neither the required number of <code>YES</code> votes to approve the proposal nor the number of <code>NO</code> votes required to reject it before the duration expires, the proposal is <code>EXPIRED</code> and <code>ProposalActions</code>\
  \ aren't carried out.\"\n        }\n      ]\n    },\n    \"ThresholdComparator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThresholdComparator\"\n        },\n        {\n          \"description\": \"Determines whether the vote percentage must be greater than the <code>ThresholdPercentage</code> or must be greater than or equal to the <code>ThreholdPercentage</code> to be approved.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-approval-threshold-policy-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: ApprovalThresholdPolicy
---
