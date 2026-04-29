---
description: ''
layout: schema
name: termsAndConditionsScalarRequest
properties_list:
- description: List of Fixed Income Security identifiers. Supported symbol types include CUSIP, SEDOL, ISIN, and FactSet Security Permanent Identifier (-S). **ID LIMIT = 250** *per request*.
  name: ids
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-terms-and-conditions-scalar-request-schema.json
slug: factset-terms-and-conditions-terms-and-conditions-scalar-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"termsAndConditionsScalarRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ids\": {\n      \"type\": \"array\",\n      \"description\": \"List of Fixed Income Security identifiers. Supported symbol types include CUSIP, SEDOL, ISIN, and FactSet Security Permanent Identifier (-S).\\n\\n**ID LIMIT = 250** *per request*.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-terms-and-conditions-scalar-request-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: termsAndConditionsScalarRequest
---
