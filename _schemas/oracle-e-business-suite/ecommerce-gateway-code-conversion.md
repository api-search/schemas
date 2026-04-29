---
description: ''
layout: schema
name: CodeConversion
properties_list:
- description: Code conversion mapping identifier
  name: codeConversionId
  type: integer
- description: Trading partner identifier
  name: tradingPartnerId
  type: integer
- description: Transaction type
  name: transactionType
  type: string
- description: Code category
  name: codeCategory
  type: string
- description: External trading partner code value
  name: externalValue
  type: string
- description: Internal Oracle EBS code value
  name: internalValue
  type: string
- description: Code conversion description
  name: description
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/ecommerce-gateway-code-conversion-schema.json
slug: ecommerce-gateway-code-conversion
source_filename: ecommerce-gateway-code-conversion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CodeConversion\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"codeConversionId\": {\n      \"type\": \"integer\",\n      \"description\": \"Code conversion mapping identifier\"\n    },\n    \"tradingPartnerId\": {\n      \"type\": \"integer\",\n      \"description\": \"Trading partner identifier\"\n    },\n    \"transactionType\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction type\"\n    },\n    \"codeCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Code category\"\n    },\n    \"externalValue\": {\n      \"type\": \"string\",\n      \"description\": \"External trading partner code value\"\n    },\n    \"internalValue\": {\n      \"type\": \"string\",\n      \"description\": \"Internal Oracle EBS code value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Code conversion description\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/ecommerce-gateway-code-conversion-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: CodeConversion
---
