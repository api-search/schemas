---
description: Schema for an SAP API Management API Product, which bundles one or more API proxies for controlled access and consumption through the developer portal.
layout: schema
name: SAP API Management API Product
properties_list:
- description: Unique identifier for the API product
  name: name
  type: string
- description: Human-readable display title in the developer portal
  name: title
  type: string
- description: Description of the API product's scope and target audience
  name: description
  type: string
- description: Visibility of the product in the developer portal
  name: scope
  type: string
- description: Publication status of the API product
  name: status
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: modifiedAt
  type: string
provider_name: SAP API Management
provider_slug: sap-api-management
schema_file: json-schema/sap-api-management-api-product-schema.json
slug: sap-api-management-api-product
source_filename: sap-api-management-api-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/sap-api-management/json-schema/api-product.json\",\n  \"title\": \"SAP API Management API Product\",\n  \"description\": \"Schema for an SAP API Management API Product, which bundles one or more API proxies for controlled access and consumption through the developer portal.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"title\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the API product\",\n      \"examples\": [\"SupplyChainAPIs\", \"finance-bundle\"]\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display title in the developer portal\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the API product's scope and target audience\"\n    },\n    \"scope\": {\n      \"type\": \"string\"\
  ,\n      \"enum\": [\"Public\", \"Private\", \"Internal\"],\n      \"description\": \"Visibility of the product in the developer portal\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Published\", \"Draft\"],\n      \"description\": \"Publication status of the API product\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-api-management/refs/heads/main/json-schema/sap-api-management-api-product-schema.json
tags:
- API Management
- Developer Portal
- Enterprise
- SAP
title: SAP API Management API Product
---
