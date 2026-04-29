---
description: A collection of log configurations.
layout: schema
name: LogConfigurations
properties_list:
- description: ''
  name: Cloudwatch
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-log-configurations-schema.json
slug: amazon-managed-blockchain-log-configurations
source_filename: amazon-managed-blockchain-log-configurations-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-log-configurations-schema.json\",\n  \"title\": \"LogConfigurations\",\n  \"description\": \"A collection of log configurations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Cloudwatch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogConfiguration\"\n        },\n        {\n          \"description\": \"Parameters for publishing logs to Amazon CloudWatch Logs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-log-configurations-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: LogConfigurations
---
