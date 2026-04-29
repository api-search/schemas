---
description: ''
layout: schema
name: Requisition
properties_list:
- description: Requisition header identifier
  name: requisitionHeaderId
  type: integer
- description: Requisition number
  name: segment1
  type: string
- description: Requisition type
  name: typeLookupCode
  type: string
- description: Authorization status
  name: authorizationStatus
  type: string
- description: Preparer identifier
  name: preparerId
  type: integer
- description: Requisition description
  name: description
  type: string
- description: ''
  name: totalAmount
  type: number
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lines
  type: array
- description: ''
  name: orgId
  type: integer
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supply-chain-requisition-schema.json
slug: supply-chain-requisition
source_filename: supply-chain-requisition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Requisition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requisitionHeaderId\": {\n      \"type\": \"integer\",\n      \"description\": \"Requisition header identifier\"\n    },\n    \"segment1\": {\n      \"type\": \"string\",\n      \"description\": \"Requisition number\"\n    },\n    \"typeLookupCode\": {\n      \"type\": \"string\",\n      \"description\": \"Requisition type\"\n    },\n    \"authorizationStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Authorization status\"\n    },\n    \"preparerId\": {\n      \"type\": \"integer\",\n      \"description\": \"Preparer identifier\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Requisition description\"\n    },\n    \"totalAmount\": {\n      \"type\": \"number\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\n    },\n    \"lines\": {\n      \"type\": \"array\"\
  \n    },\n    \"orgId\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supply-chain-requisition-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Requisition
---
