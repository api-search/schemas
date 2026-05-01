---
description: Attributes of Hyperledger Fabric for a member in a Managed Blockchain network using the Hyperledger Fabric framework.
layout: schema
name: MemberFabricAttributes
properties_list:
- description: ''
  name: AdminUsername
  type: object
- description: ''
  name: CaEndpoint
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-member-fabric-attributes-schema.json
slug: amazon-managed-blockchain-member-fabric-attributes
source_filename: amazon-managed-blockchain-member-fabric-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-member-fabric-attributes-schema.json\",\n  \"title\": \"MemberFabricAttributes\",\n  \"description\": \"Attributes of Hyperledger Fabric for a member in a Managed Blockchain network using the Hyperledger Fabric framework.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdminUsername\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameString\"\n        },\n        {\n          \"description\": \"The user name for the initial administrator user for the member.\"\n        }\n      ]\n    },\n    \"CaEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The endpoint used to access the member's certificate authority.\"\n        }\n \
  \     ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-member-fabric-attributes-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: MemberFabricAttributes
---
