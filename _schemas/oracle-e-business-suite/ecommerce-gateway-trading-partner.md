---
description: ''
layout: schema
name: TradingPartner
properties_list:
- description: Trading partner identifier
  name: tradingPartnerId
  type: integer
- description: Trading partner name
  name: tradingPartnerName
  type: string
- description: Trading partner type
  name: tradingPartnerType
  type: string
- description: Trading partner site identifier
  name: tradingPartnerSiteId
  type: integer
- description: Site name
  name: tradingPartnerSiteName
  type: string
- description: EDI location code (DUNS, DUNS+4, etc.)
  name: ediLocationCode
  type: string
- description: EDI translator code
  name: ediTranslatorCode
  type: string
- description: Document standard
  name: documentStandard
  type: string
- description: List of enabled EDI transactions for this partner
  name: enabledTransactions
  type: array
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/ecommerce-gateway-trading-partner-schema.json
slug: ecommerce-gateway-trading-partner
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TradingPartner\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tradingPartnerId\": {\n      \"type\": \"integer\",\n      \"description\": \"Trading partner identifier\"\n    },\n    \"tradingPartnerName\": {\n      \"type\": \"string\",\n      \"description\": \"Trading partner name\"\n    },\n    \"tradingPartnerType\": {\n      \"type\": \"string\",\n      \"description\": \"Trading partner type\"\n    },\n    \"tradingPartnerSiteId\": {\n      \"type\": \"integer\",\n      \"description\": \"Trading partner site identifier\"\n    },\n    \"tradingPartnerSiteName\": {\n      \"type\": \"string\",\n      \"description\": \"Site name\"\n    },\n    \"ediLocationCode\": {\n      \"type\": \"string\",\n      \"description\": \"EDI location code (DUNS, DUNS+4, etc.)\"\n    },\n    \"ediTranslatorCode\": {\n      \"type\": \"string\",\n      \"description\": \"EDI translator code\"\n  \
  \  },\n    \"documentStandard\": {\n      \"type\": \"string\",\n      \"description\": \"Document standard\"\n    },\n    \"enabledTransactions\": {\n      \"type\": \"array\",\n      \"description\": \"List of enabled EDI transactions for this partner\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/ecommerce-gateway-trading-partner-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: TradingPartner
---
