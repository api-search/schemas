---
description: Request body for updating an existing purchase order. Only provided fields will be modified.
layout: schema
name: PurchaseOrderUpdate
properties_list:
- description: Updated line items
  name: lineItems
  type: array
- description: Change request comments
  name: comments
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-purchase-order-update-schema.json
slug: sap-ariba-procurement-purchase-order-update
source_filename: sap-ariba-procurement-purchase-order-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PurchaseOrderUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating an existing purchase order. Only provided fields will be modified.\",\n  \"properties\": {\n    \"lineItems\": {\n      \"type\": \"array\",\n      \"description\": \"Updated line items\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"description\": \"Change request comments\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-purchase-order-update-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: PurchaseOrderUpdate
---
