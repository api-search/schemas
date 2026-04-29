---
description: ''
layout: schema
name: PurchaseOrder
properties_list:
- description: Purchase order header identifier
  name: poHeaderId
  type: integer
- description: Purchase order number
  name: segment1
  type: string
- description: Purchase order type
  name: typeLookupCode
  type: string
- description: Supplier/vendor identifier
  name: vendorId
  type: integer
- description: Supplier/vendor name
  name: vendorName
  type: string
- description: Vendor site identifier
  name: vendorSiteId
  type: integer
- description: Currency code (ISO 4217)
  name: currencyCode
  type: string
- description: Authorization status
  name: authorizationStatus
  type: string
- description: Approved flag
  name: approvedFlag
  type: string
- description: Close status
  name: closedCode
  type: string
- description: Total purchase order amount
  name: totalAmount
  type: number
- description: Creation date
  name: creationDate
  type: string
- description: Approval date
  name: approvedDate
  type: string
- description: Buyer employee identifier
  name: buyerId
  type: integer
- description: Ship-to location identifier
  name: shipToLocationId
  type: integer
- description: Bill-to location identifier
  name: billToLocationId
  type: integer
- description: Payment terms identifier
  name: termsId
  type: integer
- description: Purchase order description
  name: description
  type: string
- description: ''
  name: lines
  type: array
- description: Operating unit identifier
  name: orgId
  type: integer
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supply-chain-purchase-order-schema.json
slug: supply-chain-purchase-order
source_filename: supply-chain-purchase-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PurchaseOrder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"poHeaderId\": {\n      \"type\": \"integer\",\n      \"description\": \"Purchase order header identifier\"\n    },\n    \"segment1\": {\n      \"type\": \"string\",\n      \"description\": \"Purchase order number\"\n    },\n    \"typeLookupCode\": {\n      \"type\": \"string\",\n      \"description\": \"Purchase order type\"\n    },\n    \"vendorId\": {\n      \"type\": \"integer\",\n      \"description\": \"Supplier/vendor identifier\"\n    },\n    \"vendorName\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier/vendor name\"\n    },\n    \"vendorSiteId\": {\n      \"type\": \"integer\",\n      \"description\": \"Vendor site identifier\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code (ISO 4217)\"\n    },\n    \"authorizationStatus\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Authorization status\"\n    },\n    \"approvedFlag\": {\n      \"type\": \"string\",\n      \"description\": \"Approved flag\"\n    },\n    \"closedCode\": {\n      \"type\": \"string\",\n      \"description\": \"Close status\"\n    },\n    \"totalAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Total purchase order amount\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"description\": \"Creation date\"\n    },\n    \"approvedDate\": {\n      \"type\": \"string\",\n      \"description\": \"Approval date\"\n    },\n    \"buyerId\": {\n      \"type\": \"integer\",\n      \"description\": \"Buyer employee identifier\"\n    },\n    \"shipToLocationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Ship-to location identifier\"\n    },\n    \"billToLocationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Bill-to location identifier\"\n    },\n    \"termsId\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Payment terms identifier\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Purchase order description\"\n    },\n    \"lines\": {\n      \"type\": \"array\"\n    },\n    \"orgId\": {\n      \"type\": \"integer\",\n      \"description\": \"Operating unit identifier\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supply-chain-purchase-order-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: PurchaseOrder
---
