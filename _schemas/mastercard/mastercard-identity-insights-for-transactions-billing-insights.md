---
description: ''
layout: schema
name: BillingInsights
properties_list:
- description: 'The most granular level to which the address could be validated. Ex. If the address was only valid to the city level (but not to the house level), it would return valid_to_city.Possible Values are: * '
  name: validityLevel
  type: string
- description: Number of days that have passed since the address was first seen.
  name: firstSeenDays
  type: integer
- description: Number of days that have passed since the address was last seen.
  name: lastSeenDays
  type: integer
- description: 'The match status between either of the input names (person or business) and the queried entity. Possible values are: * not-found * match * no-match'
  name: matchToName
  type: string
- description: 'The relationship between billing and shipping address. Possible values are: * `match` * `city_match` * `seen_together` * `seen_with_others` * `no_relationship` * `null`'
  name: shippingAddressRelationship
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-billing-insights-schema.json
slug: mastercard-identity-insights-for-transactions-billing-insights
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BillingInsights\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"validityLevel\": {\n      \"type\": \"string\",\n      \"description\": \"The most granular level to which the address could be validated. Ex. If the address was only valid to the city level (but not to the house level), it would return valid_to_city.Possible Values are: * valid_to_house_number * missing_address * invalid * valid * valid_to_street * valid_to_country * valid_to_city * valid_to_house_number_missing_apt\"\n    },\n    \"firstSeenDays\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of days that have passed since the address was first seen.\"\n    },\n    \"lastSeenDays\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of days that have passed since the address was last seen.\"\n    },\n    \"matchToName\": {\n      \"type\": \"string\",\n      \"description\": \"The match\
  \ status between either of the input names (person or business) and the queried entity. Possible values are: * not-found * match * no-match\"\n    },\n    \"shippingAddressRelationship\": {\n      \"type\": \"string\",\n      \"description\": \"The relationship between billing and shipping address. Possible values are: * `match` * `city_match` * `seen_together` * `seen_with_others` * `no_relationship` * `null`\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-billing-insights-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: BillingInsights
---
