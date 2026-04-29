---
description: Tax calculation details for an invoice or line item
layout: schema
name: TaxDetail
properties_list:
- description: Tax code identifier
  name: taxCode
  type: string
- description: Tax category (e.g., VAT, GST, Sales Tax)
  name: taxCategory
  type: string
- description: Tax rate as a percentage
  name: taxRate
  type: number
- description: Description of the tax
  name: description
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-tax-detail-schema.json
slug: sap-ariba-procurement-tax-detail
source_filename: sap-ariba-procurement-tax-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaxDetail\",\n  \"type\": \"object\",\n  \"description\": \"Tax calculation details for an invoice or line item\",\n  \"properties\": {\n    \"taxCode\": {\n      \"type\": \"string\",\n      \"description\": \"Tax code identifier\"\n    },\n    \"taxCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Tax category (e.g., VAT, GST, Sales Tax)\"\n    },\n    \"taxRate\": {\n      \"type\": \"number\",\n      \"description\": \"Tax rate as a percentage\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the tax\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-tax-detail-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: TaxDetail
---
