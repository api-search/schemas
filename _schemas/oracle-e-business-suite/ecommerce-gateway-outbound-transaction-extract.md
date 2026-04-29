---
description: ''
layout: schema
name: OutboundTransactionExtract
properties_list:
- description: Outbound transaction type
  name: transactionType
  type: string
- description: ''
  name: tradingPartnerId
  type: integer
- description: ''
  name: tradingPartnerSiteId
  type: integer
- description: Extract documents from this date
  name: dateFrom
  type: string
- description: Extract documents to this date
  name: dateTo
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/ecommerce-gateway-outbound-transaction-extract-schema.json
slug: ecommerce-gateway-outbound-transaction-extract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OutboundTransactionExtract\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionType\": {\n      \"type\": \"string\",\n      \"description\": \"Outbound transaction type\"\n    },\n    \"tradingPartnerId\": {\n      \"type\": \"integer\"\n    },\n    \"tradingPartnerSiteId\": {\n      \"type\": \"integer\"\n    },\n    \"dateFrom\": {\n      \"type\": \"string\",\n      \"description\": \"Extract documents from this date\"\n    },\n    \"dateTo\": {\n      \"type\": \"string\",\n      \"description\": \"Extract documents to this date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/ecommerce-gateway-outbound-transaction-extract-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: OutboundTransactionExtract
---
