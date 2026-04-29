---
description: ''
layout: schema
name: ProductResource
properties_list:
- description: ''
  name: schemas
  type: array
- description: ''
  name: id
  type: string
- description: Name of product.
  name: name
  type: string
- description: Details of product.
  name: description
  type: string
- description: Description of the group the product belongs in, e.g. Exchange, Product, Database, Workstation, etc.
  name: groupDescription
  type: string
- description: A boolean representing whether the product is base-level access to FactSet, issuing the individual's serial number. Only one Product "id" per individual will have this value set to true.
  name: workstation
  type: boolean
- description: A description of the type of approval required before an order for this product can be fulfilled. This value is null for those products that do not require any approval.
  name: requiresApproval
  type: string
- description: Whether the product appears in the requester's product whitelist. Presence in the product whitelist means the requester is authorized to order this product for other users.
  name: whitelist
  type: boolean
- description: ''
  name: meta
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-procure-to-pay-scim-product-resource-schema.json
slug: factset-procure-to-pay-scim-product-resource
source_filename: factset-procure-to-pay-scim-product-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProductResource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of product.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Details of product.\"\n    },\n    \"groupDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the group the product belongs in, e.g. Exchange, Product, Database, Workstation, etc.\"\n    },\n    \"workstation\": {\n      \"type\": \"boolean\",\n      \"description\": \"A boolean representing whether the product is base-level access to FactSet, issuing the individual's serial number. Only one Product \\\"id\\\" per individual will have this value set to true.\"\n    },\n    \"requiresApproval\": {\n      \"type\": \"\
  string\",\n      \"description\": \"A description of the type of approval required before an order for this product can be fulfilled. This value is null for those products that do not require any approval.\"\n    },\n    \"whitelist\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the product appears in the requester's product whitelist. Presence in the product whitelist means the requester is authorized to order this product for other users.\"\n    },\n    \"meta\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-procure-to-pay-scim-product-resource-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ProductResource
---
