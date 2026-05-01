---
description: <p>Member configuration properties.</p> <p>Applies only to Hyperledger Fabric.</p>
layout: schema
name: Member
properties_list:
- description: ''
  name: NetworkId
  type: object
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
  name: FrameworkAttributes
  type: object
- description: ''
  name: LogPublishingConfiguration
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
schema_file: json-schema/amazon-managed-blockchain-member-schema.json
slug: amazon-managed-blockchain-member
source_filename: amazon-managed-blockchain-member-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-member-schema.json\",\n  \"title\": \"Member\",\n  \"description\": \"<p>Member configuration properties.</p> <p>Applies only to Hyperledger Fabric.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NetworkId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the network to which the member belongs.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the member.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkMemberNameString\"\
  \n        },\n        {\n          \"description\": \"The name of the member.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"An optional description for the member.\"\n        }\n      ]\n    },\n    \"FrameworkAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberFrameworkAttributes\"\n        },\n        {\n          \"description\": \"Attributes relevant to a member for the blockchain framework that the Managed Blockchain network uses.\"\n        }\n      ]\n    },\n    \"LogPublishingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberLogPublishingConfiguration\"\n        },\n        {\n          \"description\": \"Configuration properties for logging events associated with a member.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberStatus\"\n        },\n        {\n          \"description\": \"<p>The status of a member.</p> <ul> <li> <p> <code>CREATING</code> - The Amazon Web Services account is in the process of creating a member.</p> </li> <li> <p> <code>AVAILABLE</code> - The member has been created and can participate in the network.</p> </li> <li> <p> <code>CREATE_FAILED</code> - The Amazon Web Services account attempted to create a member and creation failed.</p> </li> <li> <p> <code>UPDATING</code> - The member is in the process of being updated.</p> </li> <li> <p> <code>DELETING</code> - The member and all associated resources are in the process of being deleted. Either the Amazon Web Services account that owns the member deleted it, or the member is being deleted as the result of an <code>APPROVED</code> <code>PROPOSAL</code> to remove the member.</p> </li> <li> <p> <code>DELETED</code> - The member can no longer participate on the network\
  \ and all associated resources are deleted. Either the Amazon Web Services account that owns the member deleted it, or the member is being deleted as the result of an <code>APPROVED</code> <code>PROPOSAL</code> to remove the member.</p> </li> <li> <p> <code>INACCESSIBLE_ENCRYPTION_KEY</code> - The member is impaired and might not function as expected because it cannot access the specified customer managed key in KMS for encryption at rest. Either the KMS key was disabled or deleted, or the grants on the key were revoked.</p> <p>The effect of disabling or deleting a key or of revoking a grant isn't immediate. It might take some time for the member resource to discover that the key is inaccessible. When a resource is in this state, we recommend deleting and recreating the resource.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\":\
  \ \"The date and time that the member was created.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputTagMap\"\n        },\n        {\n          \"description\": \"<p>Tags assigned to the member. Tags consist of a key and optional value.</p> <p>For more information about tags, see <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/ethereum-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Ethereum Developer Guide</i>, or <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/hyperledger-fabric-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Hyperledger Fabric Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the member.\
  \ For more information about ARNs and their format, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in the <i>Amazon Web Services General Reference</i>.\"\n        }\n      ]\n    },\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the customer managed key in Key Management Service (KMS) that the member uses for encryption at rest. If the value of this parameter is <code>\\\"AWS Owned KMS Key\\\"</code>, the member uses an Amazon Web Services owned KMS key for encryption. This parameter is inherited by the nodes that this member owns.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/hyperledger-fabric-dev/managed-blockchain-encryption-at-rest.html\\\">Encryption at Rest</a> in the <i>Amazon Managed Blockchain Hyperledger\
  \ Fabric Developer Guide</i>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-member-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: Member
---
