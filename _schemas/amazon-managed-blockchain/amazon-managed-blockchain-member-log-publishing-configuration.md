---
description: Configuration properties for logging events associated with a member of a Managed Blockchain network.
layout: schema
name: MemberLogPublishingConfiguration
properties_list:
- description: ''
  name: Fabric
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-member-log-publishing-configuration-schema.json
slug: amazon-managed-blockchain-member-log-publishing-configuration
source_filename: amazon-managed-blockchain-member-log-publishing-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-member-log-publishing-configuration-schema.json\",\n  \"title\": \"MemberLogPublishingConfiguration\",\n  \"description\": \"Configuration properties for logging events associated with a member of a Managed Blockchain network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Fabric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberFabricLogPublishingConfiguration\"\n        },\n        {\n          \"description\": \"Configuration properties for logging events associated with a member of a Managed Blockchain network using the Hyperledger Fabric framework.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-member-log-publishing-configuration-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: MemberLogPublishingConfiguration
---
