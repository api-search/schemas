---
description: Complete supplier profile on the SAP Ariba Network including company information, classifications, and qualification details
layout: schema
name: Supplier
properties_list:
- description: Unique supplier identifier (AN-ID)
  name: supplierId
  type: string
- description: Legal company name
  name: name
  type: string
- description: Trade name or DBA name
  name: doingBusinessAs
  type: string
- description: Dun and Bradstreet DUNS number
  name: dunsNumber
  type: string
- description: Tax identification number
  name: taxId
  type: string
- description: Year the company was established
  name: yearEstablished
  type: integer
- description: Employee count range
  name: numberOfEmployees
  type: string
- description: Registration status on the Ariba Network
  name: registrationStatus
  type: string
- description: UNSPSC commodity codes the supplier serves
  name: commodityCodes
  type: array
- description: Supplier certifications and compliance credentials
  name: certifications
  type: array
- description: Supplier diversity classifications
  name: diversityClassifications
  type: array
- description: Company website URL
  name: website
  type: string
- description: Company description
  name: description
  type: string
- description: Date the supplier profile was created
  name: createdDate
  type: string
- description: Date of last profile update
  name: lastModifiedDate
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-supplier-schema.json
slug: sap-ariba-procurement-supplier
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Supplier\",\n  \"type\": \"object\",\n  \"description\": \"Complete supplier profile on the SAP Ariba Network including company information, classifications, and qualification details\",\n  \"properties\": {\n    \"supplierId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique supplier identifier (AN-ID)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Legal company name\"\n    },\n    \"doingBusinessAs\": {\n      \"type\": \"string\",\n      \"description\": \"Trade name or DBA name\"\n    },\n    \"dunsNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Dun and Bradstreet DUNS number\"\n    },\n    \"taxId\": {\n      \"type\": \"string\",\n      \"description\": \"Tax identification number\"\n    },\n    \"yearEstablished\": {\n      \"type\": \"integer\",\n      \"description\": \"Year the company was established\"\n    },\n\
  \    \"numberOfEmployees\": {\n      \"type\": \"string\",\n      \"description\": \"Employee count range\"\n    },\n    \"registrationStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Registration status on the Ariba Network\"\n    },\n    \"commodityCodes\": {\n      \"type\": \"array\",\n      \"description\": \"UNSPSC commodity codes the supplier serves\"\n    },\n    \"certifications\": {\n      \"type\": \"array\",\n      \"description\": \"Supplier certifications and compliance credentials\"\n    },\n    \"diversityClassifications\": {\n      \"type\": \"array\",\n      \"description\": \"Supplier diversity classifications\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"description\": \"Company website URL\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Company description\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the supplier profile was created\"\n\
  \    },\n    \"lastModifiedDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of last profile update\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-supplier-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: Supplier
---
