---
description: ''
layout: schema
name: PurchaseOrderCreate
properties_list:
- description: ''
  name: vendorId
  type: integer
- description: ''
  name: vendorSiteId
  type: integer
- description: ''
  name: currencyCode
  type: string
- description: ''
  name: typeLookupCode
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: buyerId
  type: integer
- description: ''
  name: shipToLocationId
  type: integer
- description: ''
  name: billToLocationId
  type: integer
- description: ''
  name: termsId
  type: integer
- description: ''
  name: lines
  type: array
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supply-chain-purchase-order-create-schema.json
slug: supply-chain-purchase-order-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PurchaseOrderCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vendorId\": {\n      \"type\": \"integer\"\n    },\n    \"vendorSiteId\": {\n      \"type\": \"integer\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\"\n    },\n    \"typeLookupCode\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"buyerId\": {\n      \"type\": \"integer\"\n    },\n    \"shipToLocationId\": {\n      \"type\": \"integer\"\n    },\n    \"billToLocationId\": {\n      \"type\": \"integer\"\n    },\n    \"termsId\": {\n      \"type\": \"integer\"\n    },\n    \"lines\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supply-chain-purchase-order-create-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: PurchaseOrderCreate
---
