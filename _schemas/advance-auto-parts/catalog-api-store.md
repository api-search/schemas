---
description: An Advance Auto Parts retail store.
layout: schema
name: Store
properties_list:
- description: Store identifier.
  name: id
  type: string
- description: Store name.
  name: name
  type: string
- description: Street address.
  name: address
  type: string
- description: Phone number.
  name: phone
  type: string
- description: Business hours.
  name: hours
  type: string
- description: Distance in miles.
  name: distance
  type: number
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/catalog-api-store-schema.json
slug: catalog-api-store
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Store\",\n  \"description\": \"An Advance Auto Parts retail store.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Store identifier.\",\n      \"example\": \"store-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Store name.\",\n      \"example\": \"Advance Auto Parts - Main St\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Street address.\",\n      \"example\": \"123 Main St, Springfield, IL 62701\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number.\",\n      \"example\": \"217-555-0100\"\n    },\n    \"hours\": {\n      \"type\": \"string\",\n      \"description\": \"Business hours.\"\n    },\n    \"distance\": {\n      \"type\": \"number\",\n      \"description\": \"Distance in miles.\",\n      \"example\"\
  : 1.2\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/catalog-api-store-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: Store
---
