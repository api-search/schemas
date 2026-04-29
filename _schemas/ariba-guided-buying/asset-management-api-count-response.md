---
description: Response containing count of asset requisitions.
layout: schema
name: CountResponse
properties_list:
- description: Total count of asset requisitions.
  name: count
  type: integer
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/asset-management-api-count-response-schema.json
slug: asset-management-api-count-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/asset-management-api-count-response-schema.json\",\n  \"title\": \"CountResponse\",\n  \"description\": \"Response containing count of asset requisitions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total count of asset requisitions.\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/asset-management-api-count-response-schema.json
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: CountResponse
---
