---
description: BulkAddress schema from Adyen API
layout: schema
name: BulkAddress
properties_list:
- description: The name of the city.
  name: city
  type: string
- description: The name of the company.
  name: company
  type: string
- description: The two-character ISO-3166-1 alpha-2 country code. For example, **US**.
  name: country
  type: string
- description: The email address.
  name: email
  type: string
- description: The house number or name.
  name: houseNumberOrName
  type: string
- description: The full telephone number.
  name: mobile
  type: string
- description: 'The postal code. Maximum length: * 5 digits for addresses in the US. * 10 characters for all other countries.'
  name: postalCode
  type: string
- description: 'The two-letter ISO 3166-2 state or province code. Maximum length: 2 characters for addresses in the US.'
  name: stateOrProvince
  type: string
- description: The streetname of the house.
  name: street
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-bulk-address-schema.json
slug: notification-webhooks-bulk-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-bulk-address-schema.json\",\n  \"title\": \"BulkAddress\",\n  \"description\": \"BulkAddress schema from Adyen API\",\n  \"properties\": {\n    \"city\": {\n      \"description\": \"The name of the city.\",\n      \"type\": \"string\"\n    },\n    \"company\": {\n      \"description\": \"The name of the company.\",\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"description\": \"The two-character ISO-3166-1 alpha-2 country code. For example, **US**.\",\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"description\": \"The email address.\",\n      \"type\": \"string\"\n    },\n    \"houseNumberOrName\": {\n      \"description\": \"The house number or name.\",\n      \"type\": \"string\"\n    },\n    \"mobile\": {\n      \"description\": \"The full telephone number.\"\
  ,\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"description\": \"The postal code.\\n\\nMaximum length:\\n\\n* 5 digits for addresses in the US.\\n\\n* 10 characters for all other countries.\",\n      \"type\": \"string\"\n    },\n    \"stateOrProvince\": {\n      \"description\": \"The two-letter ISO 3166-2 state or province code.\\n\\nMaximum length: 2 characters for addresses in the US.\",\n      \"type\": \"string\"\n    },\n    \"street\": {\n      \"description\": \"The streetname of the house.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"country\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-bulk-address-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BulkAddress
---
