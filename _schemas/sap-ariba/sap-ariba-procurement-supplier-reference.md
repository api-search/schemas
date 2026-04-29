---
description: Reference to a supplier on the SAP Ariba Network
layout: schema
name: SupplierReference
properties_list:
- description: Supplier unique identifier (AN-ID on the Ariba Network or internal supplier number)
  name: supplierId
  type: string
- description: Supplier company name
  name: name
  type: string
- description: Supplier number in the ERP system
  name: erpSupplierId
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-supplier-reference-schema.json
slug: sap-ariba-procurement-supplier-reference
source_filename: sap-ariba-procurement-supplier-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SupplierReference\",\n  \"type\": \"object\",\n  \"description\": \"Reference to a supplier on the SAP Ariba Network\",\n  \"properties\": {\n    \"supplierId\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier unique identifier (AN-ID on the Ariba Network or internal supplier number)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier company name\"\n    },\n    \"erpSupplierId\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier number in the ERP system\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-supplier-reference-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: SupplierReference
---
