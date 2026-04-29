---
description: ''
layout: schema
name: BusinessPartnerBank
properties_list:
- description: Business partner number
  name: BusinessPartner
  type: string
- description: Bank detail identifier
  name: BankIdentification
  type: string
- description: Bank country key (ISO 3166-1)
  name: BankCountryKey
  type: string
- description: Bank routing number
  name: BankNumber
  type: string
- description: Bank account number
  name: BankAccount
  type: string
- description: International Bank Account Number
  name: IBAN
  type: string
- description: SWIFT/BIC code
  name: SWIFTCode
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-s4hana-cloud-business-partner-business-partner-bank-schema.json
slug: sap-s4hana-cloud-business-partner-business-partner-bank
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BusinessPartnerBank\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BusinessPartner\": {\n      \"type\": \"string\",\n      \"description\": \"Business partner number\"\n    },\n    \"BankIdentification\": {\n      \"type\": \"string\",\n      \"description\": \"Bank detail identifier\"\n    },\n    \"BankCountryKey\": {\n      \"type\": \"string\",\n      \"description\": \"Bank country key (ISO 3166-1)\"\n    },\n    \"BankNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Bank routing number\"\n    },\n    \"BankAccount\": {\n      \"type\": \"string\",\n      \"description\": \"Bank account number\"\n    },\n    \"IBAN\": {\n      \"type\": \"string\",\n      \"description\": \"International Bank Account Number\"\n    },\n    \"SWIFTCode\": {\n      \"type\": \"string\",\n      \"description\": \"SWIFT/BIC code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-s4hana-cloud-business-partner-business-partner-bank-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: BusinessPartnerBank
---
