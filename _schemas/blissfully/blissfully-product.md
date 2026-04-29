---
description: A software product in the Vendr catalog with structured attributes, features, and add-ons
layout: schema
name: Product
properties_list:
- description: Unique product identifier
  name: id
  type: string
- description: Product name
  name: name
  type: string
- description: Associated vendor identifier
  name: vendor_id
  type: string
- description: Product category
  name: category
  type: string
- description: Product description
  name: description
  type: string
- description: List of product features
  name: features
  type: array
- description: Available product add-ons
  name: add_ons
  type: array
provider_name: Blissfully
provider_slug: blissfully
schema_file: json-schema/blissfully-product-schema.json
slug: blissfully-product
source_filename: blissfully-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blissfully/refs/heads/main/json-schema/blissfully-product-schema.json\",\n  \"title\": \"Product\",\n  \"description\": \"A software product in the Vendr catalog with structured attributes, features, and add-ons\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique product identifier\",\n      \"example\": \"product-500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Product name\",\n      \"example\": \"Salesforce Sales Cloud\"\n    },\n    \"vendor_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated vendor identifier\",\n      \"example\": \"vendor-salesforce\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Product category\",\n      \"example\": \"CRM\"\n    },\n    \"description\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Product description\"\n    },\n    \"features\": {\n      \"type\": \"array\",\n      \"description\": \"List of product features\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"add_ons\": {\n      \"type\": \"array\",\n      \"description\": \"Available product add-ons\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"vendor_id\",\n    \"category\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blissfully/refs/heads/main/json-schema/blissfully-product-schema.json
tags:
- Procurement
- SaaS Discovery
- SaaS Management
- Software Procurement
- Spend Optimization
- Vendor Management
title: Product
---
