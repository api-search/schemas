---
description: A purchase requisition requesting procurement of goods or services
layout: schema
name: Requisition
properties_list:
- description: Unique requisition identifier
  name: requisitionId
  type: string
- description: Requisition title or name
  name: title
  type: string
- description: User ID of the person who created the requisition
  name: requestor
  type: string
- description: Full name of the requestor
  name: requestorName
  type: string
- description: Department of the requestor
  name: department
  type: string
- description: Company code
  name: companyCode
  type: string
- description: Desired delivery date
  name: needByDate
  type: string
- description: ''
  name: lineItems
  type: array
- description: Purchase order IDs generated from this requisition after approval
  name: purchaseOrderIds
  type: array
- description: Requisition comments
  name: comments
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: lastModifiedDate
  type: string
- description: ''
  name: approvedDate
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-requisition-schema.json
slug: sap-ariba-procurement-requisition
source_filename: sap-ariba-procurement-requisition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Requisition\",\n  \"type\": \"object\",\n  \"description\": \"A purchase requisition requesting procurement of goods or services\",\n  \"properties\": {\n    \"requisitionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique requisition identifier\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Requisition title or name\"\n    },\n    \"requestor\": {\n      \"type\": \"string\",\n      \"description\": \"User ID of the person who created the requisition\"\n    },\n    \"requestorName\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the requestor\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Department of the requestor\"\n    },\n    \"companyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Company code\"\n    },\n    \"needByDate\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Desired delivery date\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\"\n    },\n    \"purchaseOrderIds\": {\n      \"type\": \"array\",\n      \"description\": \"Purchase order IDs generated from this requisition after approval\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"description\": \"Requisition comments\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\"\n    },\n    \"lastModifiedDate\": {\n      \"type\": \"string\"\n    },\n    \"approvedDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-requisition-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: Requisition
---
