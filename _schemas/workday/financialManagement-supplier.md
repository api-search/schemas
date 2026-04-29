---
description: ''
layout: schema
name: Supplier
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: supplierName
  type: string
- description: ''
  name: supplierID
  type: string
- description: ''
  name: taxID
  type: string
- description: ''
  name: isActive
  type: boolean
- description: ''
  name: address
  type: object
provider_name: Workday
provider_slug: workday
schema_file: json-schema/financialManagement-supplier-schema.json
slug: financialManagement-supplier
source_filename: financialManagement-supplier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Supplier\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"supplierName\": {\n      \"type\": \"string\"\n    },\n    \"supplierID\": {\n      \"type\": \"string\"\n    },\n    \"taxID\": {\n      \"type\": \"string\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\"\n    },\n    \"address\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/financialManagement-supplier-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Supplier
---
