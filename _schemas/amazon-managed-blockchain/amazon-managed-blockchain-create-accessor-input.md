---
description: CreateAccessorInput schema from Amazon Managed Blockchain API
layout: schema
name: CreateAccessorInput
properties_list:
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: AccessorType
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-create-accessor-input-schema.json
slug: amazon-managed-blockchain-create-accessor-input
source_filename: amazon-managed-blockchain-create-accessor-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-create-accessor-input-schema.json\",\n  \"title\": \"CreateAccessorInput\",\n  \"description\": \"CreateAccessorInput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestTokenString\"\n        },\n        {\n          \"description\": \"This is a unique, case-sensitive identifier that you provide to ensure the idempotency of the operation. An idempotent operation completes no more than once. This identifier is required only if you make a service request directly using an HTTP client. It is generated automatically if you use an Amazon Web Services SDK or the Amazon Web Services CLI.\"\n        }\n      ]\n    },\n\
  \    \"AccessorType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessorType\"\n        },\n        {\n          \"description\": \"<p>The type of accessor.</p> <note> <p>Currently, accessor type is restricted to <code>BILLING_TOKEN</code>.</p> </note>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputTagMap\"\n        },\n        {\n          \"description\": \"<p>Tags to assign to the Accessor.</p> <p> Each tag consists of a key and an optional value. You can specify multiple key-value pairs in a single request with an overall maximum of 50 tags allowed per resource.</p> <p>For more information about tags, see <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/ethereum-dev/tagging-resources.html\\\">Tagging Resources</a> in the <i>Amazon Managed Blockchain Ethereum Developer Guide</i>, or <a href=\\\"https://docs.aws.amazon.com/managed-blockchain/latest/hyperledger-fabric-dev/tagging-resources.html\\\
  \">Tagging Resources</a> in the <i>Amazon Managed Blockchain Hyperledger Fabric Developer Guide</i>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ClientRequestToken\",\n    \"AccessorType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-create-accessor-input-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: CreateAccessorInput
---
