---
description: ''
layout: schema
name: InboundTransactionImport
properties_list:
- description: Inbound transaction type
  name: transactionType
  type: string
- description: ''
  name: tradingPartnerId
  type: integer
- description: ''
  name: tradingPartnerSiteId
  type: integer
- description: ''
  name: documentDate
  type: string
- description: Transaction-specific document data. Structure varies by transaction type (invoice, ship notice, etc.)
  name: documentData
  type: object
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/ecommerce-gateway-inbound-transaction-import-schema.json
slug: ecommerce-gateway-inbound-transaction-import
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InboundTransactionImport\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionType\": {\n      \"type\": \"string\",\n      \"description\": \"Inbound transaction type\"\n    },\n    \"tradingPartnerId\": {\n      \"type\": \"integer\"\n    },\n    \"tradingPartnerSiteId\": {\n      \"type\": \"integer\"\n    },\n    \"documentDate\": {\n      \"type\": \"string\"\n    },\n    \"documentData\": {\n      \"type\": \"object\",\n      \"description\": \"Transaction-specific document data. Structure varies by transaction type (invoice, ship notice, etc.)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/ecommerce-gateway-inbound-transaction-import-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: InboundTransactionImport
---
