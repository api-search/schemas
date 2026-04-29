---
description: ''
layout: schema
name: RequisitionLine
properties_list:
- description: ''
  name: requisitionLineId
  type: integer
- description: ''
  name: lineNum
  type: integer
- description: ''
  name: itemId
  type: integer
- description: ''
  name: itemDescription
  type: string
- description: ''
  name: categoryId
  type: integer
- description: ''
  name: quantity
  type: number
- description: ''
  name: unitMeasLookupCode
  type: string
- description: ''
  name: unitPrice
  type: number
- description: ''
  name: needByDate
  type: string
- description: ''
  name: suggestedVendorId
  type: integer
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supply-chain-requisition-line-schema.json
slug: supply-chain-requisition-line
source_filename: supply-chain-requisition-line-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequisitionLine\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requisitionLineId\": {\n      \"type\": \"integer\"\n    },\n    \"lineNum\": {\n      \"type\": \"integer\"\n    },\n    \"itemId\": {\n      \"type\": \"integer\"\n    },\n    \"itemDescription\": {\n      \"type\": \"string\"\n    },\n    \"categoryId\": {\n      \"type\": \"integer\"\n    },\n    \"quantity\": {\n      \"type\": \"number\"\n    },\n    \"unitMeasLookupCode\": {\n      \"type\": \"string\"\n    },\n    \"unitPrice\": {\n      \"type\": \"number\"\n    },\n    \"needByDate\": {\n      \"type\": \"string\"\n    },\n    \"suggestedVendorId\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supply-chain-requisition-line-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: RequisitionLine
---
