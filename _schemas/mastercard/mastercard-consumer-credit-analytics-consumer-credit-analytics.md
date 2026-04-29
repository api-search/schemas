---
description: Object containing list of customer PAN's along with score type and product type for which score will be fetched.
layout: schema
name: ConsumerCreditAnalytics
properties_list:
- description: A boolean indicating that the user of this API has requested for embedding data for the PANs. Possible value - true or false
  name: hasEmbedding
  type: boolean
- description: The 3-letter country abbreviation for the customer. These abbreviations follow https://www.iso.org/iso-3166-country-codes.html.
  name: countryCode
  type: string
- description: The card numbers and consents for which score needs to be retrieved. Max 20 PAN numbers are allowed in a request.
  name: customerPANs
  type: array
- description: Type of score needs to be retrieved for the card number, Possible value - DELINQUENCY.
  name: scoreTypes
  type: array
- description: Type of products for which score needs to be retrieved of the card number, Possible value - CREDIT_CARD.
  name: productTypes
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-consumer-credit-analytics-consumer-credit-analytics-schema.json
slug: mastercard-consumer-credit-analytics-consumer-credit-analytics
source_filename: mastercard-consumer-credit-analytics-consumer-credit-analytics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConsumerCreditAnalytics\",\n  \"type\": \"object\",\n  \"description\": \"Object containing list of customer PAN's along with score type and product type for which score will be fetched.\\n\",\n  \"properties\": {\n    \"hasEmbedding\": {\n      \"type\": \"boolean\",\n      \"description\": \"A boolean indicating that the user of this API has requested for embedding data for the PANs. Possible value - true or false\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"The 3-letter country abbreviation for the customer. These abbreviations follow https://www.iso.org/iso-3166-country-codes.html.\"\n    },\n    \"customerPANs\": {\n      \"type\": \"array\",\n      \"description\": \"The card numbers and consents for which score needs to be retrieved. Max 20 PAN numbers are allowed in a request.\"\n    },\n    \"scoreTypes\": {\n      \"type\": \"array\",\n \
  \     \"description\": \"Type of score needs to be retrieved for the card number, Possible value - DELINQUENCY.\"\n    },\n    \"productTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Type of products for which score needs to be retrieved of the card number, Possible value - CREDIT_CARD.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-consumer-credit-analytics-consumer-credit-analytics-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ConsumerCreditAnalytics
---
