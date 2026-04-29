---
description: Request body for batch asset line item updates.
layout: schema
name: BatchAssetUpdateRequest
properties_list:
- description: List of asset line item updates. Maximum 20 records.
  name: updates
  type: array
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/asset-management-api-batch-asset-update-request-schema.json
slug: asset-management-api-batch-asset-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/asset-management-api-batch-asset-update-request-schema.json\",\n  \"title\": \"BatchAssetUpdateRequest\",\n  \"description\": \"Request body for batch asset line item updates.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"updates\": {\n      \"type\": \"array\",\n      \"description\": \"List of asset line item updates. Maximum 20 records.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AssetLineItemUpdate\"\n      }\n    }\n  },\n  \"required\": [\n    \"updates\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/asset-management-api-batch-asset-update-request-schema.json
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: BatchAssetUpdateRequest
---
