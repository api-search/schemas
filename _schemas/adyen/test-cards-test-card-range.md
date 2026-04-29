---
description: TestCardRange schema from Adyen API
layout: schema
name: TestCardRange
properties_list:
- description: Contains the billing address of the card holder. The address details need to be AVS-compliant, which means that you need to provide at least street address.
  name: address
  type: object
- description: The name of the card holder, as it appears on the card, for the test card range.
  name: cardHolderName
  type: string
- description: 'The test card range security code. Example: 123'
  name: cvc
  type: string
- description: 'Expiry month for the test card range. Allowed values: * JANUARY * FEBRUARY * MARCH * APRIL * MAY * JUNE * JULY * AUGUST * SEPTEMBER * OCTOBER * NOVEMBER * DECEMBER'
  name: expiryMonth
  type: string
- description: 'Expiry year for the test card range. Example: 2020'
  name: expiryYear
  type: integer
- description: 'The last test card number in the test card range (inclusive): * Min 6, max 19 digits * BIN compliant Example: 5432 1234 1234 4321'
  name: rangeEnd
  type: string
- description: 'The first test card number in the test card range (inclusive): * Min 6, max 19 digits * BIN compliant Example: 5432 1234 1234 1234'
  name: rangeStart
  type: string
- description: '3D Secure server response. It notifies whether the specified card holder is enrolled in a 3D Secure service. Possible values: * Y (Authentication available) * N (Card holder not enrolled/not participa'
  name: threeDDirectoryServerResponse
  type: string
- description: The password used for 3D Secure authentication.
  name: threeDPassword
  type: string
- description: The username used for 3D Secure authentication.
  name: threeDUsername
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/test-cards-test-card-range-schema.json
slug: test-cards-test-card-range
source_filename: test-cards-test-card-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/test-cards-test-card-range-schema.json\",\n  \"title\": \"TestCardRange\",\n  \"description\": \"TestCardRange schema from Adyen API\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"Contains the billing address of the card holder. The address details need to be AVS-compliant, which means that you need to provide at least street address.\",\n      \"$ref\": \"#/components/schemas/AvsAddress\"\n    },\n    \"cardHolderName\": {\n      \"description\": \"The name of the card holder, as it appears on the card, for the test card range.\",\n      \"type\": \"string\"\n    },\n    \"cvc\": {\n      \"description\": \"The test card range security code.\\n\\nExample: 123\",\n      \"type\": \"string\"\n    },\n    \"expiryMonth\": {\n      \"description\": \"Expiry month for the test card range.\\n\\\
  nAllowed values:\\n* JANUARY\\n* FEBRUARY\\n* MARCH\\n* APRIL\\n* MAY\\n* JUNE\\n* JULY\\n* AUGUST\\n* SEPTEMBER\\n* OCTOBER\\n* NOVEMBER\\n* DECEMBER\",\n      \"enum\": [\n        \"APRIL\",\n        \"AUGUST\",\n        \"DECEMBER\",\n        \"FEBRUARY\",\n        \"JANUARY\",\n        \"JULY\",\n        \"JUNE\",\n        \"MARCH\",\n        \"MAY\",\n        \"NOVEMBER\",\n        \"OCTOBER\",\n        \"SEPTEMBER\"\n      ],\n      \"type\": \"string\"\n    },\n    \"expiryYear\": {\n      \"description\": \"Expiry year for the test card range.\\n\\nExample: 2020\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"rangeEnd\": {\n      \"description\": \"The last test card number in the test card range (inclusive):\\n\\n* Min 6, max 19 digits\\n* BIN compliant\\nExample: 5432 1234 1234 4321\",\n      \"type\": \"string\"\n    },\n    \"rangeStart\": {\n      \"description\": \"The first test card number in the test card range (inclusive):\\n\\n* Min 6, max\
  \ 19 digits\\n* BIN compliant\\nExample: 5432 1234 1234 1234\",\n      \"type\": \"string\"\n    },\n    \"threeDDirectoryServerResponse\": {\n      \"description\": \"3D Secure server response. It notifies whether the specified card holder is enrolled in a 3D Secure service. Possible values:\\n\\n* Y (Authentication available)\\n* N (Card holder not enrolled/not participating)\\n* U (Unable to authenticate)\",\n      \"enum\": [\n        \"N\",\n        \"U\",\n        \"Y\"\n      ],\n      \"type\": \"string\"\n    },\n    \"threeDPassword\": {\n      \"description\": \"The password used for 3D Secure authentication.\",\n      \"type\": \"string\"\n    },\n    \"threeDUsername\": {\n      \"description\": \"The username used for 3D Secure authentication.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"rangeStart\",\n    \"rangeEnd\",\n    \"expiryMonth\",\n    \"expiryYear\",\n    \"cardHolderName\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/test-cards-test-card-range-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TestCardRange
---
