---
description: CreateTestCardRangesResult schema from Adyen API
layout: schema
name: CreateTestCardRangesResult
properties_list:
- description: The results of the test card creation.
  name: rangeCreationResults
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/test-cards-create-test-card-ranges-result-schema.json
slug: test-cards-create-test-card-ranges-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/test-cards-create-test-card-ranges-result-schema.json\",\n  \"title\": \"CreateTestCardRangesResult\",\n  \"description\": \"CreateTestCardRangesResult schema from Adyen API\",\n  \"properties\": {\n    \"rangeCreationResults\": {\n      \"description\": \"The results of the test card creation.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TestCardRangeCreationResult\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"rangeCreationResults\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/test-cards-create-test-card-ranges-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreateTestCardRangesResult
---
