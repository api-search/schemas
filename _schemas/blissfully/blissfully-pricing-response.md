---
description: Pricing insights and negotiation guidance for a software product
layout: schema
name: PricingResponse
properties_list:
- description: Product identifier
  name: product_id
  type: string
- description: Fair market price per seat
  name: fair_price_per_seat
  type: number
- description: Currency code
  name: currency
  type: string
- description: Confidence level
  name: confidence
  type: string
- description: Negotiation tips
  name: negotiation_guidance
  type: string
provider_name: Blissfully
provider_slug: blissfully
schema_file: json-schema/blissfully-pricing-response-schema.json
slug: blissfully-pricing-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blissfully/refs/heads/main/json-schema/blissfully-pricing-response-schema.json\",\n  \"title\": \"PricingResponse\",\n  \"description\": \"Pricing insights and negotiation guidance for a software product\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"product_id\": {\n      \"type\": \"string\",\n      \"description\": \"Product identifier\",\n      \"example\": \"product-500123\"\n    },\n    \"fair_price_per_seat\": {\n      \"type\": \"number\",\n      \"description\": \"Fair market price per seat\",\n      \"example\": 150\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code\",\n      \"example\": \"USD\"\n    },\n    \"confidence\": {\n      \"type\": \"string\",\n      \"description\": \"Confidence level\",\n      \"enum\": [\n        \"high\",\n        \"medium\",\n        \"low\"\n   \
  \   ],\n      \"example\": \"high\"\n    },\n    \"negotiation_guidance\": {\n      \"type\": \"string\",\n      \"description\": \"Negotiation tips\",\n      \"example\": \"Consider asking for a 15-20% discount.\"\n    }\n  },\n  \"required\": [\n    \"product_id\",\n    \"fair_price_per_seat\",\n    \"currency\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blissfully/refs/heads/main/json-schema/blissfully-pricing-response-schema.json
tags:
- Procurement
- SaaS Discovery
- SaaS Management
- Software Procurement
- Spend Optimization
- Vendor Management
title: PricingResponse
---
