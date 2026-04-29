---
description: MinorUnitsMonetaryValue schema from Adyen API
layout: schema
name: MinorUnitsMonetaryValue
properties_list:
- description: The transaction amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes).
  name: amount
  type: integer
- description: The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes).
  name: currencyCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-minor-units-monetary-value-schema.json
slug: management-minor-units-monetary-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-minor-units-monetary-value-schema.json\",\n  \"title\": \"MinorUnitsMonetaryValue\",\n  \"description\": \"MinorUnitsMonetaryValue schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The transaction amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"currencyCode\": {\n      \"description\": \"The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes).\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-minor-units-monetary-value-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MinorUnitsMonetaryValue
---
