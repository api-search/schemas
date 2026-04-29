---
description: CreateAccessorOutput schema from Amazon Managed Blockchain API
layout: schema
name: CreateAccessorOutput
properties_list:
- description: ''
  name: AccessorId
  type: object
- description: ''
  name: BillingToken
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-create-accessor-output-schema.json
slug: amazon-managed-blockchain-create-accessor-output
source_filename: amazon-managed-blockchain-create-accessor-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-create-accessor-output-schema.json\",\n  \"title\": \"CreateAccessorOutput\",\n  \"description\": \"CreateAccessorOutput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the accessor.\"\n        }\n      ]\n    },\n    \"BillingToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessorBillingTokenString\"\n        },\n        {\n          \"description\": \"The billing token is a property of the Accessor. Use this token to make Ethereum API calls to your Ethereum node. The billing token is used to track\
  \ your accessor object for billing Ethereum API requests made to your Ethereum nodes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-create-accessor-output-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: CreateAccessorOutput
---
