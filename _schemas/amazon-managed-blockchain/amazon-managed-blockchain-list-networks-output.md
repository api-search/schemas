---
description: ListNetworksOutput schema from Amazon Managed Blockchain API
layout: schema
name: ListNetworksOutput
properties_list:
- description: ''
  name: Networks
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-list-networks-output-schema.json
slug: amazon-managed-blockchain-list-networks-output
source_filename: amazon-managed-blockchain-list-networks-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-list-networks-output-schema.json\",\n  \"title\": \"ListNetworksOutput\",\n  \"description\": \"ListNetworksOutput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Networks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkSummaryList\"\n        },\n        {\n          \"description\": \"An array of <code>NetworkSummary</code> objects that contain configuration properties for each network.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The pagination token that indicates the next set of results to retrieve.\"\n        }\n      ]\n  \
  \  }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-list-networks-output-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: ListNetworksOutput
---
