---
description: ListNodesOutput schema from Amazon Managed Blockchain API
layout: schema
name: ListNodesOutput
properties_list:
- description: ''
  name: Nodes
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-list-nodes-output-schema.json
slug: amazon-managed-blockchain-list-nodes-output
source_filename: amazon-managed-blockchain-list-nodes-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-list-nodes-output-schema.json\",\n  \"title\": \"ListNodesOutput\",\n  \"description\": \"ListNodesOutput schema from Amazon Managed Blockchain API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Nodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeSummaryList\"\n        },\n        {\n          \"description\": \"An array of <code>NodeSummary</code> objects that contain configuration properties for each node.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The pagination token that indicates the next set of results to retrieve.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-list-nodes-output-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: ListNodesOutput
---
