---
description: ''
layout: schema
name: SalesOrderCreate
properties_list:
- description: ''
  name: soldToOrgId
  type: integer
- description: ''
  name: orderTypeId
  type: integer
- description: ''
  name: orderedDate
  type: string
- description: ''
  name: transactionalCurrCode
  type: string
- description: ''
  name: shipToOrgId
  type: integer
- description: ''
  name: invoiceToOrgId
  type: integer
- description: ''
  name: salesrepId
  type: integer
- description: ''
  name: lines
  type: array
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supply-chain-sales-order-create-schema.json
slug: supply-chain-sales-order-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrderCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"soldToOrgId\": {\n      \"type\": \"integer\"\n    },\n    \"orderTypeId\": {\n      \"type\": \"integer\"\n    },\n    \"orderedDate\": {\n      \"type\": \"string\"\n    },\n    \"transactionalCurrCode\": {\n      \"type\": \"string\"\n    },\n    \"shipToOrgId\": {\n      \"type\": \"integer\"\n    },\n    \"invoiceToOrgId\": {\n      \"type\": \"integer\"\n    },\n    \"salesrepId\": {\n      \"type\": \"integer\"\n    },\n    \"lines\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supply-chain-sales-order-create-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: SalesOrderCreate
---
