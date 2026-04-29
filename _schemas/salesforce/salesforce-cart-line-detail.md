---
description: ''
layout: schema
name: CartLineDetail
properties_list:
- description: ''
  name: cartLineProductId
  type: string
- description: ''
  name: cartLineItemQuantity
  type: integer
- description: ''
  name: cartLineItemAmount
  type: integer
- description: ''
  name: cartLineProductCatalogId
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-cart-line-detail-schema.json
slug: salesforce-cart-line-detail
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"cartLineProductId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"cartLineItemQuantity\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"cartLineItemAmount\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"cartLineProductCatalogId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"cartLineProductId\",\n    \"cartLineItemQuantity\",\n    \"cartLineItemAmount\",\n    \"cartLineProductCatalogId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CartLineDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-cart-line-detail-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: CartLineDetail
---
