---
description: AdditionalBankIdentification schema from Adyen API
layout: schema
name: AdditionalBankIdentification
properties_list:
- description: The value of the additional bank identification.
  name: code
  type: string
- description: 'The type of additional bank identification, depending on the country. Possible values: * **gbSortCode**: The 6-digit [UK sort code](https://en.wikipedia.org/wiki/Sort_code), without separators or spac'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-additional-bank-identification-schema.json
slug: transfers-additional-bank-identification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-additional-bank-identification-schema.json\",\n  \"title\": \"AdditionalBankIdentification\",\n  \"description\": \"AdditionalBankIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"description\": \"The value of the additional bank identification.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of additional bank identification, depending on the country.\\n\\nPossible values:\\n\\n * **gbSortCode**: The 6-digit [UK sort code](https://en.wikipedia.org/wiki/Sort_code), without separators or spaces\\n * **usRoutingNumber**: The 9-digit [routing number](https://en.wikipedia.org/wiki/ABA_routing_transit_number), without separators or spaces.\",\n      \"enum\": [\n        \"gbSortCode\",\n        \"usRoutingNumber\"\
  \n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-additional-bank-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdditionalBankIdentification
---
