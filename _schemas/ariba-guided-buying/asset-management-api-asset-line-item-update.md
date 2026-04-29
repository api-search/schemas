---
description: An individual asset line item update.
layout: schema
name: AssetLineItemUpdate
properties_list:
- description: Requisition identifier.
  name: requisitionId
  type: string
- description: Line item identifier within the requisition.
  name: lineItemId
  type: string
- description: Unique asset number assigned to this line item.
  name: assetNumber
  type: string
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/asset-management-api-asset-line-item-update-schema.json
slug: asset-management-api-asset-line-item-update
source_filename: asset-management-api-asset-line-item-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/asset-management-api-asset-line-item-update-schema.json\",\n  \"title\": \"AssetLineItemUpdate\",\n  \"description\": \"An individual asset line item update.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requisitionId\": {\n      \"type\": \"string\",\n      \"description\": \"Requisition identifier.\",\n      \"example\": \"REQ-500123\"\n    },\n    \"lineItemId\": {\n      \"type\": \"string\",\n      \"description\": \"Line item identifier within the requisition.\",\n      \"example\": \"LINE-001\"\n    },\n    \"assetNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Unique asset number assigned to this line item.\",\n      \"example\": \"ASSET-001234\"\n    }\n  },\n  \"required\": [\n    \"requisitionId\",\n    \"lineItemId\",\n    \"assetNumber\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/asset-management-api-asset-line-item-update-schema.json
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: AssetLineItemUpdate
---
