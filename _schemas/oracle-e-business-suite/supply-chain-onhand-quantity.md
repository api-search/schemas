---
description: ''
layout: schema
name: OnhandQuantity
properties_list:
- description: Inventory item identifier
  name: inventoryItemId
  type: integer
- description: Organization identifier
  name: organizationId
  type: integer
- description: Subinventory code
  name: subinventoryCode
  type: string
- description: Locator identifier
  name: locatorId
  type: integer
- description: Lot number
  name: lotNumber
  type: string
- description: Serial number
  name: serialNumber
  type: string
- description: On-hand quantity
  name: transactionQuantity
  type: number
- description: Unit of measure code
  name: transactionUomCode
  type: string
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supply-chain-onhand-quantity-schema.json
slug: supply-chain-onhand-quantity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OnhandQuantity\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inventoryItemId\": {\n      \"type\": \"integer\",\n      \"description\": \"Inventory item identifier\"\n    },\n    \"organizationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization identifier\"\n    },\n    \"subinventoryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Subinventory code\"\n    },\n    \"locatorId\": {\n      \"type\": \"integer\",\n      \"description\": \"Locator identifier\"\n    },\n    \"lotNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Lot number\"\n    },\n    \"serialNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Serial number\"\n    },\n    \"transactionQuantity\": {\n      \"type\": \"number\",\n      \"description\": \"On-hand quantity\"\n    },\n    \"transactionUomCode\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Unit of measure code\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supply-chain-onhand-quantity-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: OnhandQuantity
---
