---
description: Installments schema from Adyen API
layout: schema
name: Installments
properties_list:
- description: The installment plan, used for [card installments in Japan](https://docs.adyen.com/payment-methods/cards/credit-card-installments#make-a-payment-japan). By default, this is set to **regular**. Possibl
  name: plan
  type: string
- description: Defines the number of installments. Its value needs to be greater than zero. Usually, the maximum allowed number of installments is capped. For example, it may not be possible to split a payment in mo
  name: value
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-installments-schema.json
slug: checkout-installments
source_filename: checkout-installments-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-installments-schema.json\",\n  \"title\": \"Installments\",\n  \"description\": \"Installments schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"plan\": {\n      \"x-addedInVersion\": \"64\",\n      \"description\": \"The installment plan, used for [card installments in Japan](https://docs.adyen.com/payment-methods/cards/credit-card-installments#make-a-payment-japan). By default, this is set to **regular**. Possible values:\\n* **regular**\\n* **revolving**\\n\",\n      \"enum\": [\n        \"regular\",\n        \"revolving\"\n      ],\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Defines the number of installments. Its value needs to be greater than zero.\\n\\nUsually, the maximum allowed number of installments is capped. For example, it may\
  \ not be possible to split a payment in more than 24 installments. The acquirer sets this upper limit, so its value may vary.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-installments-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Installments
---
