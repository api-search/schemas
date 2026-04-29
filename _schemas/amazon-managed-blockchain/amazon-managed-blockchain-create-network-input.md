---
description: CreateNetworkInput schema from Amazon Managed Blockchain API
layout: schema
name: CreateNetworkInput
properties_list:
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Framework
  type: object
- description: ''
  name: FrameworkVersion
  type: object
- description: ''
  name: FrameworkConfiguration
  type: object
- description: ''
  name: VotingPolicy
  type: object
- description: ''
  name: MemberConfiguration
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-create-network-input-schema.json
slug: amazon-managed-blockchain-create-network-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-create-network-input-schema.json\",\n  \"title\": \"CreateNetworkInput\",\n  \"description\": \"CreateNetworkInput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestTokenString\"\n        },\n        {\n          \"description\": \"This is a unique, case-sensitive identifier that you provide to ensure the idempotency of the operation. An idempotent operation completes no more than once. This identifier is required only if you make a service request directly using an HTTP client. It is generated automatically if you use an Amazon Web Services SDK or the Amazon Web Services CLI. \"\n        }\n      ]\n    },\n\
  \    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the network.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"An optional description for the network.\"\n        }\n      ]\n    },\n    \"Framework\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Framework\"\n        },\n        {\n          \"description\": \"The blockchain framework that the network uses.\"\n        }\n      ]\n    },\n    \"FrameworkVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrameworkVersionString\"\n        },\n        {\n          \"description\": \"The version of the blockchain framework that the network uses.\"\n        }\n      ]\n    },\n    \"FrameworkConfiguration\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkFrameworkConfiguration\"\n        },\n        {\n          \"description\": \" Configuration properties of the blockchain framework relevant to the network configuration. \"\n        }\n      ]\n    },\n    \"VotingPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VotingPolicy\"\n        },\n        {\n          \"description\": \" The voting rules used by the network to determine if a proposal is approved. \"\n        }\n      ]\n    },\n    \"MemberConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberConfiguration\"\n        },\n        {\n          \"description\": \"Configuration properties for the first member within the network.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputTagMap\"\n        },\n        {\n          \"description\":\
  \ \"<p>Tags to assign to the network.</p> <p> Each tag consists of a key and an optional value. You can specify multiple key-value pairs in a single request with an overall maximum of 50 tags allowed per resource.</p> <p>For more information about tags, see <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/ethereum-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Ethereum Developer Guide</i>, or <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/hyperledger-fabric-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Hyperledger Fabric Developer Guide</i>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ClientRequestToken\",\n    \"Name\",\n    \"Framework\",\n    \"FrameworkVersion\",\n    \"VotingPolicy\",\n    \"MemberConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-create-network-input-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: CreateNetworkInput
---
