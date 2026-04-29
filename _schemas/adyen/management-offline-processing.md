---
description: OfflineProcessing schema from Adyen API
layout: schema
name: OfflineProcessing
properties_list:
- description: The maximum offline transaction amount for chip cards, in the processing currency and specified in [minor units](https://docs.adyen.com/development-resources/currency-codes).
  name: chipFloorLimit
  type: integer
- description: The maximum offline transaction amount for swiped cards, in the specified currency.
  name: offlineSwipeLimits
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-offline-processing-schema.json
slug: management-offline-processing
source_filename: management-offline-processing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-offline-processing-schema.json\",\n  \"title\": \"OfflineProcessing\",\n  \"description\": \"OfflineProcessing schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"chipFloorLimit\": {\n      \"description\": \"The maximum offline transaction amount for chip cards, in the processing currency and specified in [minor units](https://docs.adyen.com/development-resources/currency-codes).\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"offlineSwipeLimits\": {\n      \"description\": \"The maximum offline transaction amount for swiped cards, in the specified currency.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MinorUnitsMonetaryValue\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-offline-processing-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: OfflineProcessing
---
