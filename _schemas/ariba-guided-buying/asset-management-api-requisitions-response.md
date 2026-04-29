---
description: Response containing a list of asset requisitions.
layout: schema
name: RequisitionsResponse
properties_list:
- description: Total count of requisitions.
  name: count
  type: integer
- description: List of requisitions with asset line items.
  name: requisitions
  type: array
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/asset-management-api-requisitions-response-schema.json
slug: asset-management-api-requisitions-response
source_filename: asset-management-api-requisitions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/asset-management-api-requisitions-response-schema.json\",\n  \"title\": \"RequisitionsResponse\",\n  \"description\": \"Response containing a list of asset requisitions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total count of requisitions.\",\n      \"example\": 1\n    },\n    \"requisitions\": {\n      \"type\": \"array\",\n      \"description\": \"List of requisitions with asset line items.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Requisition\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/asset-management-api-requisitions-response-schema.json
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: RequisitionsResponse
---
