---
description: ''
layout: schema
name: InboundTransaction
properties_list:
- description: Transaction identifier
  name: transactionId
  type: integer
- description: Inbound transaction type code
  name: transactionType
  type: string
- description: Transaction description
  name: transactionDescription
  type: string
- description: Document standard (X12 or EDIFACT)
  name: documentStandard
  type: string
- description: ASC X12 document number (810, 832, 843, 856, 857)
  name: documentNumber
  type: string
- description: Trading partner identifier
  name: tradingPartnerId
  type: integer
- description: ''
  name: tradingPartnerName
  type: string
- description: ''
  name: tradingPartnerSiteId
  type: integer
- description: Processing status
  name: processStatus
  type: string
- description: Document date
  name: documentDate
  type: string
- description: Document total amount
  name: documentAmount
  type: number
- description: Currency code
  name: currencyCode
  type: string
- description: Error message if processing failed
  name: errorMessage
  type: string
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/ecommerce-gateway-inbound-transaction-schema.json
slug: ecommerce-gateway-inbound-transaction
source_filename: ecommerce-gateway-inbound-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InboundTransaction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"integer\",\n      \"description\": \"Transaction identifier\"\n    },\n    \"transactionType\": {\n      \"type\": \"string\",\n      \"description\": \"Inbound transaction type code\"\n    },\n    \"transactionDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction description\"\n    },\n    \"documentStandard\": {\n      \"type\": \"string\",\n      \"description\": \"Document standard (X12 or EDIFACT)\"\n    },\n    \"documentNumber\": {\n      \"type\": \"string\",\n      \"description\": \"ASC X12 document number (810, 832, 843, 856, 857)\"\n    },\n    \"tradingPartnerId\": {\n      \"type\": \"integer\",\n      \"description\": \"Trading partner identifier\"\n    },\n    \"tradingPartnerName\": {\n      \"type\": \"string\"\n    },\n    \"tradingPartnerSiteId\"\
  : {\n      \"type\": \"integer\"\n    },\n    \"processStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Processing status\"\n    },\n    \"documentDate\": {\n      \"type\": \"string\",\n      \"description\": \"Document date\"\n    },\n    \"documentAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Document total amount\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Error message if processing failed\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/ecommerce-gateway-inbound-transaction-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: InboundTransaction
---
