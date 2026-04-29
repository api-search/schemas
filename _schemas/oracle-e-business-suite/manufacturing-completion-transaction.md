---
description: ''
layout: schema
name: CompletionTransaction
properties_list:
- description: WIP entity identifier
  name: wipEntityId
  type: integer
- description: Organization identifier
  name: organizationId
  type: integer
- description: Completion quantity
  name: transactionQuantity
  type: number
- description: Transaction unit of measure
  name: transactionUom
  type: string
- description: Completion subinventory
  name: subinventoryCode
  type: string
- description: Completion locator
  name: locatorId
  type: integer
- description: Transaction date
  name: transactionDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/manufacturing-completion-transaction-schema.json
slug: manufacturing-completion-transaction
source_filename: manufacturing-completion-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompletionTransaction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"wipEntityId\": {\n      \"type\": \"integer\",\n      \"description\": \"WIP entity identifier\"\n    },\n    \"organizationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization identifier\"\n    },\n    \"transactionQuantity\": {\n      \"type\": \"number\",\n      \"description\": \"Completion quantity\"\n    },\n    \"transactionUom\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction unit of measure\"\n    },\n    \"subinventoryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Completion subinventory\"\n    },\n    \"locatorId\": {\n      \"type\": \"integer\",\n      \"description\": \"Completion locator\"\n    },\n    \"transactionDate\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/manufacturing-completion-transaction-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: CompletionTransaction
---
