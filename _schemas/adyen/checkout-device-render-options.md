---
description: DeviceRenderOptions schema from Adyen API
layout: schema
name: DeviceRenderOptions
properties_list:
- description: 'Supported SDK interface types. Allowed values: * native * html * both'
  name: sdkInterface
  type: string
- description: 'UI types supported for displaying specific challenges. Allowed values: * text * singleSelect * outOfBand * otherHtml * multiSelect'
  name: sdkUiType
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-device-render-options-schema.json
slug: checkout-device-render-options
source_filename: checkout-device-render-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-device-render-options-schema.json\",\n  \"title\": \"DeviceRenderOptions\",\n  \"description\": \"DeviceRenderOptions schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sdkInterface\": {\n      \"default\": \"both\",\n      \"description\": \"Supported SDK interface types.\\nAllowed values:\\n* native\\n* html\\n* both\",\n      \"enum\": [\n        \"native\",\n        \"html\",\n        \"both\"\n      ],\n      \"type\": \"string\"\n    },\n    \"sdkUiType\": {\n      \"description\": \"UI types supported for displaying specific challenges.\\nAllowed values:\\n* text\\n* singleSelect\\n* outOfBand\\n* otherHtml\\n* multiSelect\",\n      \"items\": {\n        \"enum\": [\n          \"multiSelect\",\n          \"otherHtml\",\n          \"outOfBand\",\n          \"singleSelect\"\
  ,\n          \"text\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-device-render-options-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DeviceRenderOptions
---
