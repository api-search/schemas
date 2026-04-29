---
description: Payment terms governing when and how invoices should be paid
layout: schema
name: PaymentTerms
properties_list:
- description: Payment terms code
  name: code
  type: string
- description: Human-readable payment terms description
  name: description
  type: string
- description: Number of days until payment is due
  name: netDays
  type: integer
- description: Early payment discount percentage
  name: discountPercent
  type: number
- description: Number of days within which discount applies
  name: discountDays
  type: integer
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-payment-terms-schema.json
slug: sap-ariba-procurement-payment-terms
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaymentTerms\",\n  \"type\": \"object\",\n  \"description\": \"Payment terms governing when and how invoices should be paid\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Payment terms code\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable payment terms description\"\n    },\n    \"netDays\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of days until payment is due\"\n    },\n    \"discountPercent\": {\n      \"type\": \"number\",\n      \"description\": \"Early payment discount percentage\"\n    },\n    \"discountDays\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of days within which discount applies\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-payment-terms-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: PaymentTerms
---
