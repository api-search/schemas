---
description: ''
layout: schema
name: MaterialTransaction
properties_list:
- description: WIP entity identifier
  name: wipEntityId
  type: integer
- description: Organization identifier
  name: organizationId
  type: integer
- description: Operation sequence number
  name: operationSeqNum
  type: integer
- description: Inventory item identifier
  name: inventoryItemId
  type: integer
- description: Transaction quantity (positive=issue, negative=return)
  name: transactionQuantity
  type: number
- description: Transaction unit of measure
  name: transactionUom
  type: string
- description: Transaction type
  name: transactionType
  type: string
- description: Source/destination subinventory
  name: subinventoryCode
  type: string
- description: Locator identifier
  name: locatorId
  type: integer
- description: Transaction date
  name: transactionDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/manufacturing-material-transaction-schema.json
slug: manufacturing-material-transaction
source_filename: manufacturing-material-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MaterialTransaction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"wipEntityId\": {\n      \"type\": \"integer\",\n      \"description\": \"WIP entity identifier\"\n    },\n    \"organizationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization identifier\"\n    },\n    \"operationSeqNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Operation sequence number\"\n    },\n    \"inventoryItemId\": {\n      \"type\": \"integer\",\n      \"description\": \"Inventory item identifier\"\n    },\n    \"transactionQuantity\": {\n      \"type\": \"number\",\n      \"description\": \"Transaction quantity (positive=issue, negative=return)\"\n    },\n    \"transactionUom\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction unit of measure\"\n    },\n    \"transactionType\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction\
  \ type\"\n    },\n    \"subinventoryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Source/destination subinventory\"\n    },\n    \"locatorId\": {\n      \"type\": \"integer\",\n      \"description\": \"Locator identifier\"\n    },\n    \"transactionDate\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/manufacturing-material-transaction-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: MaterialTransaction
---
