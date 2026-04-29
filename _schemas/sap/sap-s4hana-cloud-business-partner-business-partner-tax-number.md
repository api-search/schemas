---
description: ''
layout: schema
name: BusinessPartnerTaxNumber
properties_list:
- description: Business partner number
  name: BusinessPartner
  type: string
- description: Tax number category
  name: BPTaxType
  type: string
- description: Tax identification number
  name: BPTaxNumber
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-s4hana-cloud-business-partner-business-partner-tax-number-schema.json
slug: sap-s4hana-cloud-business-partner-business-partner-tax-number
source_filename: sap-s4hana-cloud-business-partner-business-partner-tax-number-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BusinessPartnerTaxNumber\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BusinessPartner\": {\n      \"type\": \"string\",\n      \"description\": \"Business partner number\"\n    },\n    \"BPTaxType\": {\n      \"type\": \"string\",\n      \"description\": \"Tax number category\"\n    },\n    \"BPTaxNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Tax identification number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-s4hana-cloud-business-partner-business-partner-tax-number-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: BusinessPartnerTaxNumber
---
