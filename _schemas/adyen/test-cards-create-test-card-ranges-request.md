---
description: CreateTestCardRangesRequest schema from Adyen API
layout: schema
name: CreateTestCardRangesRequest
properties_list:
- description: The code of the account, for which the test card ranges should be created.
  name: accountCode
  type: string
- description: 'The type of the account, for which the test card ranges should be created. Permitted values: * Company * MerchantAccount > These values are case-sensitive.'
  name: accountTypeCode
  type: string
- description: A list of test card ranges to create.
  name: testCardRanges
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/test-cards-create-test-card-ranges-request-schema.json
slug: test-cards-create-test-card-ranges-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/test-cards-create-test-card-ranges-request-schema.json\",\n  \"title\": \"CreateTestCardRangesRequest\",\n  \"description\": \"CreateTestCardRangesRequest schema from Adyen API\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the account, for which the test card ranges should be created.\",\n      \"type\": \"string\"\n    },\n    \"accountTypeCode\": {\n      \"description\": \"The type of the account, for which the test card ranges should be created.\\n\\nPermitted values:\\n* Company\\n* MerchantAccount\\n> These values are case-sensitive.\",\n      \"type\": \"string\"\n    },\n    \"testCardRanges\": {\n      \"description\": \"A list of test card ranges to create.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TestCardRange\"\n      },\n      \"type\"\
  : \"array\"\n    }\n  },\n  \"required\": [\n    \"accountTypeCode\",\n    \"accountCode\",\n    \"testCardRanges\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/test-cards-create-test-card-ranges-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreateTestCardRangesRequest
---
