---
description: ''
layout: schema
name: Ip
properties_list:
- description: The distance (in miles) between the IP address and the physical address.
  name: billingAddressDistance
  type: integer
- description: Number of days that have passed since the IP address was last seen.
  name: lastSeenDays
  type: integer
- description: 'Ip Connection type description. Possible values are: * cable-dsl * corporate * cellular * dialup'
  name: connectionType
  type: string
- description: The distance (in miles) between the IP address and the physical address.
  name: shippingAddressDistance
  type: integer
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-ip-schema.json
slug: mastercard-identity-insights-for-transactions-ip
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Ip\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billingAddressDistance\": {\n      \"type\": \"integer\",\n      \"description\": \"The distance (in miles) between the IP address and the physical address.\"\n    },\n    \"lastSeenDays\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of days that have passed since the IP address was last seen.\"\n    },\n    \"connectionType\": {\n      \"type\": \"string\",\n      \"description\": \"Ip Connection type description. Possible values are: * cable-dsl * corporate * cellular * dialup\"\n    },\n    \"shippingAddressDistance\": {\n      \"type\": \"integer\",\n      \"description\": \"The distance (in miles) between the IP address and the physical address.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-ip-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Ip
---
