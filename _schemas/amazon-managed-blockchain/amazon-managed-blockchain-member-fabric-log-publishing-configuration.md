---
description: Configuration properties for logging events associated with a member of a Managed Blockchain network using the Hyperledger Fabric framework.
layout: schema
name: MemberFabricLogPublishingConfiguration
properties_list:
- description: ''
  name: CaLogs
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-member-fabric-log-publishing-configuration-schema.json
slug: amazon-managed-blockchain-member-fabric-log-publishing-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-member-fabric-log-publishing-configuration-schema.json\",\n  \"title\": \"MemberFabricLogPublishingConfiguration\",\n  \"description\": \"Configuration properties for logging events associated with a member of a Managed Blockchain network using the Hyperledger Fabric framework.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CaLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogConfigurations\"\n        },\n        {\n          \"description\": \"Configuration properties for logging events associated with a member's Certificate Authority (CA). CA logs help you determine when a member in your account joins the network, or when new peers register with a member CA.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-member-fabric-log-publishing-configuration-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: MemberFabricLogPublishingConfiguration
---
