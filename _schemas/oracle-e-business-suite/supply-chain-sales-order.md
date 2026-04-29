---
description: ''
layout: schema
name: SalesOrder
properties_list:
- description: Order header identifier
  name: headerId
  type: integer
- description: Order number
  name: orderNumber
  type: integer
- description: Order date
  name: orderedDate
  type: string
- description: Order type identifier
  name: orderTypeId
  type: integer
- description: Order type name
  name: orderTypeName
  type: string
- description: Customer identifier (sold-to)
  name: soldToOrgId
  type: integer
- description: Customer name
  name: customerName
  type: string
- description: Ship-to organization identifier
  name: shipToOrgId
  type: integer
- description: Bill-to organization identifier
  name: invoiceToOrgId
  type: integer
- description: Transaction currency code (ISO 4217)
  name: transactionalCurrCode
  type: string
- description: Order flow status
  name: flowStatusCode
  type: string
- description: ''
  name: bookedFlag
  type: string
- description: Order total amount
  name: totalAmount
  type: number
- description: Salesperson identifier
  name: salesrepId
  type: integer
- description: ''
  name: lines
  type: array
- description: ''
  name: orgId
  type: integer
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supply-chain-sales-order-schema.json
slug: supply-chain-sales-order
source_filename: supply-chain-sales-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"headerId\": {\n      \"type\": \"integer\",\n      \"description\": \"Order header identifier\"\n    },\n    \"orderNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Order number\"\n    },\n    \"orderedDate\": {\n      \"type\": \"string\",\n      \"description\": \"Order date\"\n    },\n    \"orderTypeId\": {\n      \"type\": \"integer\",\n      \"description\": \"Order type identifier\"\n    },\n    \"orderTypeName\": {\n      \"type\": \"string\",\n      \"description\": \"Order type name\"\n    },\n    \"soldToOrgId\": {\n      \"type\": \"integer\",\n      \"description\": \"Customer identifier (sold-to)\"\n    },\n    \"customerName\": {\n      \"type\": \"string\",\n      \"description\": \"Customer name\"\n    },\n    \"shipToOrgId\": {\n      \"type\": \"integer\",\n      \"description\": \"Ship-to\
  \ organization identifier\"\n    },\n    \"invoiceToOrgId\": {\n      \"type\": \"integer\",\n      \"description\": \"Bill-to organization identifier\"\n    },\n    \"transactionalCurrCode\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction currency code (ISO 4217)\"\n    },\n    \"flowStatusCode\": {\n      \"type\": \"string\",\n      \"description\": \"Order flow status\"\n    },\n    \"bookedFlag\": {\n      \"type\": \"string\"\n    },\n    \"totalAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Order total amount\"\n    },\n    \"salesrepId\": {\n      \"type\": \"integer\",\n      \"description\": \"Salesperson identifier\"\n    },\n    \"lines\": {\n      \"type\": \"array\"\n    },\n    \"orgId\": {\n      \"type\": \"integer\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supply-chain-sales-order-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: SalesOrder
---
