---
description: InternalCategoryData schema from Adyen API
layout: schema
name: InternalCategoryData
properties_list:
- description: The capture's merchant reference included in the transfer.
  name: modificationMerchantReference
  type: string
- description: The capture reference included in the transfer.
  name: modificationPspReference
  type: string
- description: '**internal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-internal-category-data-schema.json
slug: transfers-internal-category-data
source_filename: transfers-internal-category-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-internal-category-data-schema.json\",\n  \"title\": \"InternalCategoryData\",\n  \"description\": \"InternalCategoryData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"modificationMerchantReference\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The capture's merchant reference included in the transfer.\",\n      \"type\": \"string\"\n    },\n    \"modificationPspReference\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The capture reference included in the transfer.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"internal\",\n      \"description\": \"**internal**\",\n      \"enum\": [\n        \"internal\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-internal-category-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: InternalCategoryData
---
