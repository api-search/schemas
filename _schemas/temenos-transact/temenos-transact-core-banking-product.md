---
description: A banking product definition from the product catalog
layout: schema
name: Product
properties_list:
- description: Unique product identifier
  name: productId
  type: string
- description: Name of the product
  name: productName
  type: string
- description: Product group classification
  name: productGroup
  type: string
- description: Detailed product description
  name: description
  type: string
- description: Supported currencies
  name: currency
  type: array
- description: Interest rate conditions
  name: interestRate
  type: object
- description: Minimum balance requirement
  name: minimumBalance
  type: number
- description: Associated fees and charges
  name: fees
  type: array
- description: Product availability status
  name: status
  type: string
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-product-schema.json
slug: temenos-transact-core-banking-product
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Product\",\n  \"type\": \"object\",\n  \"description\": \"A banking product definition from the product catalog\",\n  \"properties\": {\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique product identifier\"\n    },\n    \"productName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the product\"\n    },\n    \"productGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Product group classification\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed product description\"\n    },\n    \"currency\": {\n      \"type\": \"array\",\n      \"description\": \"Supported currencies\"\n    },\n    \"interestRate\": {\n      \"type\": \"object\",\n      \"description\": \"Interest rate conditions\"\n    },\n    \"minimumBalance\": {\n      \"type\": \"number\",\n      \"description\": \"Minimum\
  \ balance requirement\"\n    },\n    \"fees\": {\n      \"type\": \"array\",\n      \"description\": \"Associated fees and charges\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Product availability status\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-product-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: Product
---
