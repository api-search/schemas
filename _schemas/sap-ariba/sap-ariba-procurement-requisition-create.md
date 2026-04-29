---
description: Request body for creating a new requisition
layout: schema
name: RequisitionCreate
properties_list:
- description: ''
  name: title
  type: string
- description: ''
  name: needByDate
  type: string
- description: ''
  name: companyCode
  type: string
- description: ''
  name: lineItems
  type: array
- description: ''
  name: comments
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-requisition-create-schema.json
slug: sap-ariba-procurement-requisition-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequisitionCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new requisition\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"needByDate\": {\n      \"type\": \"string\"\n    },\n    \"companyCode\": {\n      \"type\": \"string\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\"\n    },\n    \"comments\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-requisition-create-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: RequisitionCreate
---
