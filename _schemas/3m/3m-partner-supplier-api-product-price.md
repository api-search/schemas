---
description: Pricing information for a specific 3M product
layout: schema
name: ProductPrice
properties_list:
- description: Unique product identifier
  name: productId
  type: string
- description: Partner-negotiated unit price
  name: unitPrice
  type: number
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Pricing tier applied to this partner
  name: pricingTier
  type: string
- description: Date when this pricing becomes effective
  name: effectiveDate
  type: string
- description: Date when this pricing expires
  name: expirationDate
  type: string
provider_name: 3M
provider_slug: 3m
schema_file: json-schema/3m-partner-supplier-api-product-price-schema.json
slug: 3m-partner-supplier-api-product-price
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-product-price-schema.json\",\n  \"title\": \"ProductPrice\",\n  \"description\": \"Pricing information for a specific 3M product\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique product identifier\",\n      \"example\": \"PROD-12345\"\n    },\n    \"unitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Partner-negotiated unit price\",\n      \"example\": 24.99\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code (ISO 4217)\",\n      \"example\": \"USD\"\n    },\n    \"pricingTier\": {\n      \"type\": \"string\",\n      \"description\": \"Pricing tier applied to this partner\",\n      \"example\": \"partner\"\n    },\n    \"effectiveDate\": {\n    \
  \  \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when this pricing becomes effective\",\n      \"example\": \"2025-01-01\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when this pricing expires\",\n      \"example\": \"2025-12-31\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-product-price-schema.json
tags:
- Industrial
- Manufacturing
- Supply Chain
title: ProductPrice
---
