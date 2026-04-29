---
description: EntryModesRestriction schema from Adyen API
layout: schema
name: EntryModesRestriction
properties_list:
- description: Defines how the condition must be evaluated.
  name: operation
  type: string
- description: 'List of point-of-sale entry modes. Possible values: **barcode**, **chip**, **cof**, **contactless**, **magstripe**, **manual**, **ocr**, **server**.'
  name: value
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-entry-modes-restriction-schema.json
slug: configuration-entry-modes-restriction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-entry-modes-restriction-schema.json\",\n  \"title\": \"EntryModesRestriction\",\n  \"description\": \"EntryModesRestriction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"description\": \"Defines how the condition must be evaluated.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"List of point-of-sale entry modes.\\n\\nPossible values: **barcode**, **chip**, **cof**, **contactless**, **magstripe**, **manual**, **ocr**, **server**.\\n\\n\",\n      \"items\": {\n        \"enum\": [\n          \"barcode\",\n          \"chip\",\n          \"cof\",\n          \"contactless\",\n          \"magstripe\",\n          \"manual\",\n          \"ocr\",\n          \"server\",\n          \"unknown\"\n        ],\n        \"type\"\
  : \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"operation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-entry-modes-restriction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: EntryModesRestriction
---
