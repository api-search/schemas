---
description: Paginated list of purchase order line items
layout: schema
name: LineItemListResponse
properties_list:
- description: Total number of line items
  name: totalCount
  type: integer
- description: Number of records skipped
  name: skip
  type: integer
- description: Maximum records per page
  name: limit
  type: integer
- description: ''
  name: lineItems
  type: array
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-line-item-list-response-schema.json
slug: sap-ariba-procurement-line-item-list-response
source_filename: sap-ariba-procurement-line-item-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LineItemListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of purchase order line items\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of line items\"\n    },\n    \"skip\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of records skipped\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum records per page\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-line-item-list-response-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: LineItemListResponse
---
