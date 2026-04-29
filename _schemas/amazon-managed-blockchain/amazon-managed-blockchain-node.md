---
description: Configuration properties of a node.
layout: schema
name: Node
properties_list:
- description: ''
  name: NetworkId
  type: object
- description: ''
  name: MemberId
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: InstanceType
  type: object
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: FrameworkAttributes
  type: object
- description: ''
  name: LogPublishingConfiguration
  type: object
- description: ''
  name: StateDB
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
- description: ''
  name: KmsKeyArn
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-node-schema.json
slug: amazon-managed-blockchain-node
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-node-schema.json\",\n  \"title\": \"Node\",\n  \"description\": \"Configuration properties of a node.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NetworkId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the network that the node is on.\"\n        }\n      ]\n    },\n    \"MemberId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"<p>The unique identifier of the member to which the node belongs.</p> <p>Applies only to Hyperledger Fabric.</p>\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the node.\"\n        }\n      ]\n    },\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceTypeString\"\n        },\n        {\n          \"description\": \"The instance type of the node.\"\n        }\n      ]\n    },\n    \"AvailabilityZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailabilityZoneString\"\n        },\n        {\n          \"description\": \"The Availability Zone in which the node exists. Required for Ethereum nodes. \"\n        }\n      ]\n    },\n    \"FrameworkAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeFrameworkAttributes\"\n        },\n        {\n          \"description\": \"Attributes of the blockchain framework being used.\"\n        }\n      ]\n    },\n    \"LogPublishingConfiguration\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeLogPublishingConfiguration\"\n        },\n        {\n          \"description\": \"Configuration properties for logging events associated with a peer node on a Hyperledger Fabric network on Managed Blockchain.\"\n        }\n      ]\n    },\n    \"StateDB\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateDBType\"\n        },\n        {\n          \"description\": \"<p>The state database that the node uses. Values are <code>LevelDB</code> or <code>CouchDB</code>.</p> <p>Applies only to Hyperledger Fabric.</p>\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the node.</p> <ul> <li> <p> <code>CREATING</code> - The Amazon Web Services account is in the process of creating a node.</p> </li> <li> <p> <code>AVAILABLE</code> - The\
  \ node has been created and can participate in the network.</p> </li> <li> <p> <code>UNHEALTHY</code> - The node is impaired and might not function as expected. Amazon Managed Blockchain automatically finds nodes in this state and tries to recover them. If a node is recoverable, it returns to <code>AVAILABLE</code>. Otherwise, it moves to <code>FAILED</code> status.</p> </li> <li> <p> <code>CREATE_FAILED</code> - The Amazon Web Services account attempted to create a node and creation failed.</p> </li> <li> <p> <code>UPDATING</code> - The node is in the process of being updated.</p> </li> <li> <p> <code>DELETING</code> - The node is in the process of being deleted.</p> </li> <li> <p> <code>DELETED</code> - The node can no longer participate on the network.</p> </li> <li> <p> <code>FAILED</code> - The node is no longer functional, cannot be recovered, and must be deleted.</p> </li> <li> <p> <code>INACCESSIBLE_ENCRYPTION_KEY</code> - The node is impaired and might not function as expected\
  \ because it cannot access the specified customer managed key in KMS for encryption at rest. Either the KMS key was disabled or deleted, or the grants on the key were revoked.</p> <p>The effect of disabling or deleting a key or of revoking a grant isn't immediate. It might take some time for the node resource to discover that the key is inaccessible. When a resource is in this state, we recommend deleting and recreating the resource.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time that the node was created.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputTagMap\"\n        },\n        {\n          \"description\": \"<p>Tags assigned to the node. Each tag consists of a key and optional value.</p> <p>For more information about tags,\
  \ see <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/ethereum-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Ethereum Developer Guide</i>, or <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/hyperledger-fabric-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Hyperledger Fabric Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the node. For more information about ARNs and their format, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in the <i>Amazon Web Services General Reference</i>.\"\n        }\n      ]\n    },\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the customer managed key in Key Management Service (KMS) that the node uses for encryption at rest. If the value of this parameter is <code>\\\"AWS Owned KMS Key\\\"</code>, the node uses an Amazon Web Services owned KMS key for encryption. The node inherits this parameter from the member that it belongs to.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/hyperledger-fabric-dev/managed-blockchain-encryption-at-rest.html\\\">Encryption at Rest</a> in the <i>Amazon Managed Blockchain Hyperledger Fabric Developer Guide</i>.</p> <p>Applies only to Hyperledger Fabric.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-node-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: Node
---
