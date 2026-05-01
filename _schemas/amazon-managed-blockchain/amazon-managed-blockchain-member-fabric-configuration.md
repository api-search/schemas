---
description: Configuration properties for Hyperledger Fabric for a member in a Managed Blockchain network that is using the Hyperledger Fabric framework.
layout: schema
name: MemberFabricConfiguration
properties_list:
- description: ''
  name: AdminUsername
  type: object
- description: ''
  name: AdminPassword
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-member-fabric-configuration-schema.json
slug: amazon-managed-blockchain-member-fabric-configuration
source_filename: amazon-managed-blockchain-member-fabric-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-member-fabric-configuration-schema.json\",\n  \"title\": \"MemberFabricConfiguration\",\n  \"description\": \"Configuration properties for Hyperledger Fabric for a member in a Managed Blockchain network that is using the Hyperledger Fabric framework.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdminUsername\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameString\"\n        },\n        {\n          \"description\": \"The user name for the member's initial administrative user.\"\n        }\n      ]\n    },\n    \"AdminPassword\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PasswordString\"\n        },\n        {\n          \"description\": \"The password for the member's initial administrative\
  \ user. The <code>AdminPassword</code> must be at least 8 characters long and no more than 32 characters. It must contain at least one uppercase letter, one lowercase letter, and one digit. It cannot have a single quotation mark (\\u2018), a double quotation marks (\\u201c), a forward slash(/), a backward slash(\\\\), @, or a space.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AdminUsername\",\n    \"AdminPassword\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-member-fabric-configuration-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: MemberFabricConfiguration
---
