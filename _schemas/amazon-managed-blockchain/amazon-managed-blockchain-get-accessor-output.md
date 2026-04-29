---
description: GetAccessorOutput schema from Amazon Managed Blockchain API
layout: schema
name: GetAccessorOutput
properties_list:
- description: ''
  name: Accessor
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-get-accessor-output-schema.json
slug: amazon-managed-blockchain-get-accessor-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-get-accessor-output-schema.json\",\n  \"title\": \"GetAccessorOutput\",\n  \"description\": \"GetAccessorOutput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Accessor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Accessor\"\n        },\n        {\n          \"description\": \"The properties of the accessor.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-get-accessor-output-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: GetAccessorOutput
---
