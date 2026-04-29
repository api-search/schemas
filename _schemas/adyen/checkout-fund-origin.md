---
description: FundOrigin schema from Adyen API
layout: schema
name: FundOrigin
properties_list:
- description: The address where to send the invoice.
  name: billingAddress
  type: object
- description: Email address of the person.
  name: shopperEmail
  type: string
- description: The name of the person
  name: shopperName
  type: object
- description: Phone number of the person
  name: telephoneNumber
  type: string
- description: ''
  name: walletIdentifier
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-fund-origin-schema.json
slug: checkout-fund-origin
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-fund-origin-schema.json\",\n  \"title\": \"FundOrigin\",\n  \"description\": \"FundOrigin schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billingAddress\": {\n      \"description\": \"The address where to send the invoice.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"Email address of the person.\",\n      \"type\": \"string\"\n    },\n    \"shopperName\": {\n      \"description\": \"The name of the person\",\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n    \"telephoneNumber\": {\n      \"description\": \"Phone number of the person\",\n      \"type\": \"string\"\n    },\n    \"walletIdentifier\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-fund-origin-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: FundOrigin
---
