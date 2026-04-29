---
description: Network configuration properties.
layout: schema
name: Network
properties_list:
- description: ''
  name: Id
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
  name: FrameworkAttributes
  type: object
- description: ''
  name: VpcEndpointServiceName
  type: object
- description: ''
  name: VotingPolicy
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Arn
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-network-schema.json
slug: amazon-managed-blockchain-network
source_filename: amazon-managed-blockchain-network-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-network-schema.json\",\n  \"title\": \"Network\",\n  \"description\": \"Network configuration properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the network.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the network.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"Attributes\
  \ of the blockchain framework for the network.\"\n        }\n      ]\n    },\n    \"Framework\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Framework\"\n        },\n        {\n          \"description\": \"The blockchain framework that the network uses.\"\n        }\n      ]\n    },\n    \"FrameworkVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrameworkVersionString\"\n        },\n        {\n          \"description\": \"The version of the blockchain framework that the network uses.\"\n        }\n      ]\n    },\n    \"FrameworkAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkFrameworkAttributes\"\n        },\n        {\n          \"description\": \"Attributes of the blockchain framework that the network uses.\"\n        }\n      ]\n    },\n    \"VpcEndpointServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n      \
  \  },\n        {\n          \"description\": \"The VPC endpoint service name of the VPC endpoint service of the network. Members use the VPC endpoint service name to create a VPC endpoint to access network resources.\"\n        }\n      ]\n    },\n    \"VotingPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VotingPolicy\"\n        },\n        {\n          \"description\": \"The voting rules that the network uses to decide if a proposal is accepted.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkStatus\"\n        },\n        {\n          \"description\": \"The current status of the network.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time that the network was created.\"\n        }\n      ]\n    },\n    \"\
  Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputTagMap\"\n        },\n        {\n          \"description\": \"<p>Tags assigned to the network. Each tag consists of a key and optional value.</p> <p>For more information about tags, see <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/ethereum-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Ethereum Developer Guide</i>, or <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/hyperledger-fabric-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Hyperledger Fabric Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the network. For more information about ARNs and their format, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\
  \">Amazon Resource Names (ARNs)</a> in the <i>Amazon Web Services General Reference</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-network-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: Network
---
