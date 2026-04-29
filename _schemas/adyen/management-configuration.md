---
description: Configuration schema from Adyen API
layout: schema
name: Configuration
properties_list:
- description: Payment method, like **eftpos_australia** or **mc**. See the [possible values](https://docs.adyen.com/development-resources/paymentmethodvariant#management-api).
  name: brand
  type: string
- description: Countries, to filter different surcharge amounts for domestic or international cards.
  name: country
  type: array
- description: Currency, and surcharge percentage or amount.
  name: currencies
  type: array
- description: 'Funding source. Possible values: * **Credit** * **Debit**'
  name: sources
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-configuration-schema.json
slug: management-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-configuration-schema.json\",\n  \"title\": \"Configuration\",\n  \"description\": \"Configuration schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"description\": \"Payment method, like **eftpos_australia** or **mc**. See the [possible values](https://docs.adyen.com/development-resources/paymentmethodvariant#management-api). \",\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"description\": \"Countries, to filter different surcharge amounts for domestic or international cards.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"currencies\": {\n      \"description\": \"Currency, and surcharge percentage or amount.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Currency\"\
  \n      },\n      \"type\": \"array\"\n    },\n    \"sources\": {\n      \"description\": \"Funding source. Possible values:\\n* **Credit**\\n* **Debit**\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"brand\",\n    \"currencies\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-configuration-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Configuration
---
