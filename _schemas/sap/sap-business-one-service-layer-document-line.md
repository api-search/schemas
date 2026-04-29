---
description: ''
layout: schema
name: DocumentLine
properties_list:
- description: Item code
  name: ItemCode
  type: string
- description: Ordered quantity
  name: Quantity
  type: number
- description: Price per unit
  name: UnitPrice
  type: number
- description: Line currency
  name: Currency
  type: string
- description: Warehouse code for the line item
  name: WarehouseCode
  type: string
- description: Tax code applied to the line
  name: TaxCode
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-business-one-service-layer-document-line-schema.json
slug: sap-business-one-service-layer-document-line
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DocumentLine\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ItemCode\": {\n      \"type\": \"string\",\n      \"description\": \"Item code\"\n    },\n    \"Quantity\": {\n      \"type\": \"number\",\n      \"description\": \"Ordered quantity\"\n    },\n    \"UnitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Price per unit\"\n    },\n    \"Currency\": {\n      \"type\": \"string\",\n      \"description\": \"Line currency\"\n    },\n    \"WarehouseCode\": {\n      \"type\": \"string\",\n      \"description\": \"Warehouse code for the line item\"\n    },\n    \"TaxCode\": {\n      \"type\": \"string\",\n      \"description\": \"Tax code applied to the line\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-business-one-service-layer-document-line-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: DocumentLine
---
