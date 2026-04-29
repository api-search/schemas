---
description: Paginated list of receipts
layout: schema
name: ReceiptListResponse
properties_list:
- description: ''
  name: totalCount
  type: integer
- description: ''
  name: skip
  type: integer
- description: ''
  name: limit
  type: integer
- description: ''
  name: receipts
  type: array
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-receipt-list-response-schema.json
slug: sap-ariba-procurement-receipt-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReceiptListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of receipts\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\"\n    },\n    \"skip\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"receipts\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-receipt-list-response-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: ReceiptListResponse
---
