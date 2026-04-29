---
description: Vendor or merchant information for an expense
layout: schema
name: Vendor
properties_list:
- description: The vendor identifier
  name: id
  type: string
- description: The vendor or merchant name
  name: name
  type: string
- description: Additional vendor description
  name: description
  type: string
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-vendor-schema.json
slug: sap-concur-expense-vendor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Vendor\",\n  \"type\": \"object\",\n  \"description\": \"Vendor or merchant information for an expense\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The vendor identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The vendor or merchant name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Additional vendor description\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-vendor-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: Vendor
---
