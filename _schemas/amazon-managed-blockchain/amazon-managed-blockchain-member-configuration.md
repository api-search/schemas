---
description: <p>Configuration properties of the member.</p> <p>Applies only to Hyperledger Fabric.</p>
layout: schema
name: MemberConfiguration
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: FrameworkConfiguration
  type: object
- description: ''
  name: LogPublishingConfiguration
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: KmsKeyArn
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-member-configuration-schema.json
slug: amazon-managed-blockchain-member-configuration
source_filename: amazon-managed-blockchain-member-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-member-configuration-schema.json\",\n  \"title\": \"MemberConfiguration\",\n  \"description\": \"<p>Configuration properties of the member.</p> <p>Applies only to Hyperledger Fabric.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkMemberNameString\"\n        },\n        {\n          \"description\": \"The name of the member.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"An optional description of the member.\"\n        }\n      ]\n    },\n    \"FrameworkConfiguration\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/MemberFrameworkConfiguration\"\n        },\n        {\n          \"description\": \"Configuration properties of the blockchain framework relevant to the member.\"\n        }\n      ]\n    },\n    \"LogPublishingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberLogPublishingConfiguration\"\n        },\n        {\n          \"description\": \"Configuration properties for logging events associated with a member of a Managed Blockchain network.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputTagMap\"\n        },\n        {\n          \"description\": \"<p>Tags assigned to the member. Tags consist of a key and optional value. </p> <p>When specifying tags during creation, you can specify multiple key-value pairs in a single request, with an overall maximum of 50 tags added to each resource.</p> <p>For more information about tags,\
  \ see <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/ethereum-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Ethereum Developer Guide</i>, or <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/hyperledger-fabric-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Hyperledger Fabric Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnString\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the customer managed key in Key Management Service (KMS) to use for encryption at rest in the member. This parameter is inherited by any nodes that this member creates. For more information, see <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/hyperledger-fabric-dev/managed-blockchain-encryption-at-rest.html\\\">Encryption at Rest</a>\
  \ in the <i>Amazon Managed Blockchain Hyperledger Fabric Developer Guide</i>.</p> <p>Use one of the following options to specify this parameter:</p> <ul> <li> <p> <b>Undefined or empty string</b> - By default, use an KMS key that is owned and managed by Amazon Web Services on your behalf.</p> </li> <li> <p> <b>A valid symmetric customer managed KMS key</b> - Use the specified KMS key in your account that you create, own, and manage.</p> <p>Amazon Managed Blockchain doesn't support asymmetric keys. For more information, see <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/symmetric-asymmetric.html\\\">Using symmetric and asymmetric keys</a> in the <i>Key Management Service Developer Guide</i>.</p> <p>The following is an example of a KMS key ARN: <code>arn:aws:kms:us-east-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"FrameworkConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-member-configuration-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: MemberConfiguration
---
