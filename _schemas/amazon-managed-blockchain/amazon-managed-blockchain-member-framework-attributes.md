---
description: Attributes relevant to a member for the blockchain framework that the Managed Blockchain network uses.
layout: schema
name: MemberFrameworkAttributes
properties_list:
- description: ''
  name: Fabric
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-member-framework-attributes-schema.json
slug: amazon-managed-blockchain-member-framework-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-member-framework-attributes-schema.json\",\n  \"title\": \"MemberFrameworkAttributes\",\n  \"description\": \"Attributes relevant to a member for the blockchain framework that the Managed Blockchain network uses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Fabric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberFabricAttributes\"\n        },\n        {\n          \"description\": \"Attributes of Hyperledger Fabric relevant to a member on a Managed Blockchain network that uses Hyperledger Fabric.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-member-framework-attributes-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: MemberFrameworkAttributes
---
