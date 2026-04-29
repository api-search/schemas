---
description: ''
layout: schema
name: EnabledTransaction
properties_list:
- description: Transaction type code
  name: transactionType
  type: string
- description: Transaction description
  name: transactionDescription
  type: string
- description: Transaction direction
  name: direction
  type: string
- description: ASC X12 or EDIFACT document identifier
  name: documentId
  type: string
- description: Whether transaction is enabled
  name: enabled
  type: boolean
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/ecommerce-gateway-enabled-transaction-schema.json
slug: ecommerce-gateway-enabled-transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnabledTransaction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionType\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction type code\"\n    },\n    \"transactionDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction description\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction direction\"\n    },\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"ASC X12 or EDIFACT document identifier\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether transaction is enabled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/ecommerce-gateway-enabled-transaction-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: EnabledTransaction
---
