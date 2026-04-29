---
description: An asset line item on a requisition.
layout: schema
name: AssetLineItem
properties_list:
- description: Line item identifier.
  name: lineItemId
  type: string
- description: Line item description.
  name: description
  type: string
- description: Asset category classification.
  name: assetCategory
  type: string
- description: Quantity ordered.
  name: quantity
  type: integer
- description: Assigned asset number (populated after update).
  name: assetNumber
  type: string
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/asset-management-api-asset-line-item-schema.json
slug: asset-management-api-asset-line-item
source_filename: asset-management-api-asset-line-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/asset-management-api-asset-line-item-schema.json\",\n  \"title\": \"AssetLineItem\",\n  \"description\": \"An asset line item on a requisition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lineItemId\": {\n      \"type\": \"string\",\n      \"description\": \"Line item identifier.\",\n      \"example\": \"LINE-001\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Line item description.\",\n      \"example\": \"Laptop Computer\"\n    },\n    \"assetCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Asset category classification.\",\n      \"example\": \"IT Equipment\"\n    },\n    \"quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity ordered.\",\n      \"example\": 1\n    },\n    \"assetNumber\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"Assigned asset number (populated after update).\",\n      \"example\": \"ASSET-001234\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/asset-management-api-asset-line-item-schema.json
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: AssetLineItem
---
