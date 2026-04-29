---
description: Paginated list of suppliers
layout: schema
name: SupplierListResponse
properties_list:
- description: Total number of matching suppliers
  name: totalCount
  type: integer
- description: Number of records skipped
  name: skip
  type: integer
- description: Maximum records per page
  name: limit
  type: integer
- description: ''
  name: suppliers
  type: array
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-supplier-list-response-schema.json
slug: sap-ariba-procurement-supplier-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SupplierListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of suppliers\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching suppliers\"\n    },\n    \"skip\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of records skipped\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum records per page\"\n    },\n    \"suppliers\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-supplier-list-response-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: SupplierListResponse
---
