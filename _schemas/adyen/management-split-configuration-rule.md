---
description: SplitConfigurationRule schema from Adyen API
layout: schema
name: SplitConfigurationRule
properties_list:
- description: The currency condition that defines whether the split logic applies. Its value must be a three-character [ISO currency code](https://en.wikipedia.org/wiki/ISO_4217).
  name: currency
  type: string
- description: 'The funding source condition of the payment method (only for cards). Possible values: **credit**, **debit**, or **ANY**.'
  name: fundingSource
  type: string
- description: 'The payment method condition that defines whether the split logic applies. Possible values: * [Payment method variant](https://docs.adyen.com/development-resources/paymentmethodvariant): Apply the spl'
  name: paymentMethod
  type: string
- description: The unique identifier of the split configuration rule.
  name: ruleId
  type: string
- description: 'The sales channel condition that defines whether the split logic applies. Possible values: * **Ecommerce**: Online transactions where the cardholder is present. * **ContAuth**: Card on file and/or sub'
  name: shopperInteraction
  type: string
- description: Contains the split logic that is applied if the rule conditions are met.
  name: splitLogic
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-split-configuration-rule-schema.json
slug: management-split-configuration-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-split-configuration-rule-schema.json\",\n  \"title\": \"SplitConfigurationRule\",\n  \"description\": \"SplitConfigurationRule schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"description\": \"The currency condition that defines whether the split logic applies.\\nIts value must be a three-character [ISO currency code](https://en.wikipedia.org/wiki/ISO_4217).\",\n      \"type\": \"string\"\n    },\n    \"fundingSource\": {\n      \"description\": \"The funding source condition of the payment method (only for cards).\\n\\nPossible values: **credit**, **debit**, or **ANY**.\",\n      \"enum\": [\n        \"credit\",\n        \"debit\",\n        \"ANY\"\n      ],\n      \"type\": \"string\"\n    },\n    \"paymentMethod\": {\n      \"description\": \"The\
  \ payment method condition that defines whether the split logic applies.\\n\\nPossible values:\\n* [Payment method variant](https://docs.adyen.com/development-resources/paymentmethodvariant): Apply the split logic for a specific payment method.\\n* **ANY**: Apply the split logic for all available payment methods.\",\n      \"type\": \"string\"\n    },\n    \"ruleId\": {\n      \"description\": \"The unique identifier of the split configuration rule.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"shopperInteraction\": {\n      \"description\": \"The sales channel condition that defines whether the split logic applies.\\n\\nPossible values:\\n* **Ecommerce**: Online transactions where the cardholder is present.\\n* **ContAuth**: Card on file and/or subscription transactions, where the cardholder is known to the merchant (returning customer).\\n* **Moto**: Mail-order and telephone-order transactions where the customer is in contact with the merchant via email or\
  \ telephone.\\n* **POS**: Point-of-sale transactions where the customer is physically present to make a payment using a secure payment terminal.\\n* **ANY**: All sales channels.\",\n      \"enum\": [\n        \"Ecommerce\",\n        \"ContAuth\",\n        \"Moto\",\n        \"POS\",\n        \"ANY\"\n      ],\n      \"type\": \"string\"\n    },\n    \"splitLogic\": {\n      \"description\": \"Contains the split logic that is applied if the rule conditions are met.\",\n      \"$ref\": \"#/components/schemas/SplitConfigurationLogic\"\n    }\n  },\n  \"required\": [\n    \"paymentMethod\",\n    \"shopperInteraction\",\n    \"currency\",\n    \"splitLogic\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-split-configuration-rule-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SplitConfigurationRule
---
