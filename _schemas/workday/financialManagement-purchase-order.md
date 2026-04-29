---
description: ''
layout: schema
name: PurchaseOrder
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: purchaseOrderNumber
  type: string
- description: ''
  name: orderDate
  type: string
- description: ''
  name: totalAmount
  type: number
- description: ''
  name: status
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/financialManagement-purchase-order-schema.json
slug: financialManagement-purchase-order
source_filename: financialManagement-purchase-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PurchaseOrder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"purchaseOrderNumber\": {\n      \"type\": \"string\"\n    },\n    \"orderDate\": {\n      \"type\": \"string\"\n    },\n    \"totalAmount\": {\n      \"type\": \"number\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/financialManagement-purchase-order-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: PurchaseOrder
---
