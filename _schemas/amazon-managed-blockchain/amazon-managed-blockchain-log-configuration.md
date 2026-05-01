---
description: A configuration for logging events.
layout: schema
name: LogConfiguration
properties_list:
- description: ''
  name: Enabled
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-log-configuration-schema.json
slug: amazon-managed-blockchain-log-configuration
source_filename: amazon-managed-blockchain-log-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-log-configuration-schema.json\",\n  \"title\": \"LogConfiguration\",\n  \"description\": \"A configuration for logging events.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Enabled\"\n        },\n        {\n          \"description\": \"Indicates whether logging is enabled.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-log-configuration-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: LogConfiguration
---
