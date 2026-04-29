---
description: UpdateMemberInput schema from Amazon Managed Blockchain API
layout: schema
name: UpdateMemberInput
properties_list:
- description: ''
  name: LogPublishingConfiguration
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-update-member-input-schema.json
slug: amazon-managed-blockchain-update-member-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-update-member-input-schema.json\",\n  \"title\": \"UpdateMemberInput\",\n  \"description\": \"UpdateMemberInput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogPublishingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberLogPublishingConfiguration\"\n        },\n        {\n          \"description\": \"Configuration properties for publishing to Amazon CloudWatch Logs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-update-member-input-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: UpdateMemberInput
---
