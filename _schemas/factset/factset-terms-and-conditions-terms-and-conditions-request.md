---
description: ''
layout: schema
name: termsAndConditionsRequest
properties_list:
- description: List of Fixed Income Security identifiers. Supported symbol types include CUSIP, SEDOL, ISIN, and FactSet Security Permanent Identifier (-S). **ID LIMIT = 250** *per request*.
  name: ids
  type: array
- description: List of Terms and Conditions data items.
  name: fields
  type: array
- description: Selects the Fixed Income metrics by major category - * **SECURITY_DETAILS** = Detailed information about the security. * **COUPON_DETAILS** = Coupon details. * **CONVERTIBLE_FEATURES** = Features of c
  name: categories
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-terms-and-conditions-request-schema.json
slug: factset-terms-and-conditions-terms-and-conditions-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"termsAndConditionsRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ids\": {\n      \"type\": \"array\",\n      \"description\": \"List of Fixed Income Security identifiers. Supported symbol types include CUSIP, SEDOL, ISIN, and FactSet Security Permanent Identifier (-S).\\n\\n**ID LIMIT = 250** *per request*.\\n\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"List of Terms and Conditions data items.\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\": \"Selects the Fixed Income metrics by major category -\\n* **SECURITY_DETAILS** = Detailed information about the security.\\n* **COUPON_DETAILS** = Coupon details.\\n* **CONVERTIBLE_FEATURES** = Features of convertible instruments.\\n* **REDEMPTION_OPTIONS** = Redemption options.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-terms-and-conditions-request-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: termsAndConditionsRequest
---
