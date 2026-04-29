---
description: A data integration flow definition
layout: schema
name: DataIntegrationFlow
properties_list:
- description: The instance identifier
  name: instanceId
  type: string
- description: The flow name
  name: name
  type: string
- description: Data sources for the flow
  name: sources
  type: array
- description: Data transformation configuration
  name: transformation
  type: object
- description: Data target configuration
  name: target
  type: object
- description: Creation timestamp
  name: createdTime
  type: string
- description: Last modification timestamp
  name: lastModifiedTime
  type: string
provider_name: Amazon Supply Chain
provider_slug: amazon-supply-chain
schema_file: json-schema/amazon-supply-chain-data-integration-flow-schema.json
slug: amazon-supply-chain-data-integration-flow
source_filename: amazon-supply-chain-data-integration-flow-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/json-schema/amazon-supply-chain-data-integration-flow-schema.json\",\n  \"title\": \"DataIntegrationFlow\",\n  \"description\": \"A data integration flow definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The instance identifier\",\n      \"example\": \"inst-abc12345\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The flow name\",\n      \"example\": \"MyIntegrationFlow\"\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"description\": \"Data sources for the flow\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"transformation\": {\n      \"type\": \"object\",\n      \"description\": \"Data transformation configuration\"\n    },\n    \"target\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"Data target configuration\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp\"\n    },\n    \"lastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/json-schema/amazon-supply-chain-data-integration-flow-schema.json
tags:
- AWS
- ERP Integration
- Logistics
- Machine Learning
- Supply Chain
title: DataIntegrationFlow
---
