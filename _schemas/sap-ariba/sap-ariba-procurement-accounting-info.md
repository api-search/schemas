---
description: Accounting assignment information for cost allocation on purchase order line items
layout: schema
name: AccountingInfo
properties_list:
- description: Cost center identifier for expenditure allocation
  name: costCenter
  type: string
- description: General ledger account number
  name: generalLedger
  type: string
- description: Fixed asset number
  name: asset
  type: string
- description: Internal order number
  name: internalOrder
  type: string
- description: Work Breakdown Structure element
  name: wbsElement
  type: string
- description: Percentage of line item amount allocated to this accounting assignment
  name: percentage
  type: number
- description: SAP distribution indicator flag
  name: sapDistributionFlag
  type: string
- description: Account assignment category code for the line item expenditure
  name: accountCategory
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-accounting-info-schema.json
slug: sap-ariba-procurement-accounting-info
source_filename: sap-ariba-procurement-accounting-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountingInfo\",\n  \"type\": \"object\",\n  \"description\": \"Accounting assignment information for cost allocation on purchase order line items\",\n  \"properties\": {\n    \"costCenter\": {\n      \"type\": \"string\",\n      \"description\": \"Cost center identifier for expenditure allocation\"\n    },\n    \"generalLedger\": {\n      \"type\": \"string\",\n      \"description\": \"General ledger account number\"\n    },\n    \"asset\": {\n      \"type\": \"string\",\n      \"description\": \"Fixed asset number\"\n    },\n    \"internalOrder\": {\n      \"type\": \"string\",\n      \"description\": \"Internal order number\"\n    },\n    \"wbsElement\": {\n      \"type\": \"string\",\n      \"description\": \"Work Breakdown Structure element\"\n    },\n    \"percentage\": {\n      \"type\": \"number\",\n      \"description\": \"Percentage of line item amount allocated to this accounting\
  \ assignment\"\n    },\n    \"sapDistributionFlag\": {\n      \"type\": \"string\",\n      \"description\": \"SAP distribution indicator flag\"\n    },\n    \"accountCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Account assignment category code for the line item expenditure\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-accounting-info-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: AccountingInfo
---
