---
description: TestCardRangeCreationResult schema from Adyen API
layout: schema
name: TestCardRangeCreationResult
properties_list:
- description: 'The last test card number in the generated test card range. Example: 5432 1234 1234 4321'
  name: cardNumberRangeEnd
  type: string
- description: 'The first test card number in the generated test card range. Example: 5432 1234 1234 1234'
  name: cardNumberRangeStart
  type: string
- description: 'Notification message. It informs about the outcome of the operation. Possible values: * CREATED * ALREADY_EXISTS * ERROR'
  name: creationResultCode
  type: string
- description: An optional information message about the result.
  name: message
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/test-cards-test-card-range-creation-result-schema.json
slug: test-cards-test-card-range-creation-result
source_filename: test-cards-test-card-range-creation-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/test-cards-test-card-range-creation-result-schema.json\",\n  \"title\": \"TestCardRangeCreationResult\",\n  \"description\": \"TestCardRangeCreationResult schema from Adyen API\",\n  \"properties\": {\n    \"cardNumberRangeEnd\": {\n      \"description\": \"The last test card number in the generated test card range.\\n\\nExample: 5432 1234 1234 4321\",\n      \"type\": \"string\"\n    },\n    \"cardNumberRangeStart\": {\n      \"description\": \"The first test card number in the generated test card range.\\n\\nExample: 5432 1234 1234 1234\",\n      \"type\": \"string\"\n    },\n    \"creationResultCode\": {\n      \"description\": \"Notification message. It informs about the outcome of the operation. Possible values:\\n* CREATED\\n* ALREADY_EXISTS\\n* ERROR\",\n      \"enum\": [\n        \"ALREADY_EXISTS\",\n  \
  \      \"CREATED\",\n        \"ERROR\"\n      ],\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"description\": \"An optional information message about the result.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"cardNumberRangeStart\",\n    \"cardNumberRangeEnd\",\n    \"creationResultCode\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/test-cards-test-card-range-creation-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TestCardRangeCreationResult
---
