---
description: ''
layout: schema
name: OutboundTransaction
properties_list:
- description: Transaction identifier
  name: transactionId
  type: integer
- description: Outbound transaction type code
  name: transactionType
  type: string
- description: Transaction description
  name: transactionDescription
  type: string
- description: Document standard (X12 or EDIFACT)
  name: documentStandard
  type: string
- description: ASC X12/EDIFACT document number
  name: documentNumber
  type: string
- description: ''
  name: tradingPartnerId
  type: integer
- description: ''
  name: tradingPartnerName
  type: string
- description: ''
  name: tradingPartnerSiteId
  type: integer
- description: ''
  name: processStatus
  type: string
- description: Source document identifier in Oracle EBS
  name: sourceDocumentId
  type: integer
- description: Source document number
  name: sourceDocumentNumber
  type: string
- description: ''
  name: documentDate
  type: string
- description: ''
  name: documentAmount
  type: number
- description: ''
  name: currencyCode
  type: string
- description: ''
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
schema_file: json-schema/ecommerce-gateway-outbound-transaction-schema.json
slug: ecommerce-gateway-outbound-transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OutboundTransaction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"integer\",\n      \"description\": \"Transaction identifier\"\n    },\n    \"transactionType\": {\n      \"type\": \"string\",\n      \"description\": \"Outbound transaction type code\"\n    },\n    \"transactionDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction description\"\n    },\n    \"documentStandard\": {\n      \"type\": \"string\",\n      \"description\": \"Document standard (X12 or EDIFACT)\"\n    },\n    \"documentNumber\": {\n      \"type\": \"string\",\n      \"description\": \"ASC X12/EDIFACT document number\"\n    },\n    \"tradingPartnerId\": {\n      \"type\": \"integer\"\n    },\n    \"tradingPartnerName\": {\n      \"type\": \"string\"\n    },\n    \"tradingPartnerSiteId\": {\n      \"type\": \"integer\"\n    },\n    \"processStatus\"\
  : {\n      \"type\": \"string\"\n    },\n    \"sourceDocumentId\": {\n      \"type\": \"integer\",\n      \"description\": \"Source document identifier in Oracle EBS\"\n    },\n    \"sourceDocumentNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Source document number\"\n    },\n    \"documentDate\": {\n      \"type\": \"string\"\n    },\n    \"documentAmount\": {\n      \"type\": \"number\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/ecommerce-gateway-outbound-transaction-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: OutboundTransaction
---
