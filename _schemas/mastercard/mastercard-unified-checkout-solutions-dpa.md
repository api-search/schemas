---
description: An array of objects to contain DPA registration details.
layout: schema
name: Dpa
properties_list:
- description: 'Card networks that are supported for DPA registration. The following networks are supported: MASTERCARD, VISA, DISCOVER, AMEX.'
  name: supportedCardBrands
  type: array
- description: 'A flag for the Integrator to indicate that they would not like to have their Cardholder''s debit cards tokenized. Conditional: Must be set to true when the Digital Payment Application (DPA) processes i'
  name: debitTokenRequested
  type: boolean
- description: List of checkout types to be supported by the DPA. These include CLICK_TO_PAY, GUEST_CHECKOUT_TOKENIZATION and CARD_ON_FILE_TOKENIZATION.
  name: supportedCheckoutTypes
  type: array
- description: ''
  name: acquirerData
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-unified-checkout-solutions-dpa-schema.json
slug: mastercard-unified-checkout-solutions-dpa
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Dpa\",\n  \"type\": \"object\",\n  \"description\": \"An array of objects to contain DPA registration details.\",\n  \"properties\": {\n    \"supportedCardBrands\": {\n      \"type\": \"array\",\n      \"description\": \"Card networks that are supported for DPA registration. The following networks are supported: MASTERCARD, VISA, DISCOVER, AMEX.\\n\"\n    },\n    \"debitTokenRequested\": {\n      \"type\": \"boolean\",\n      \"description\": \"A flag for the Integrator to indicate that they would not like to have their Cardholder's debit cards tokenized.\\n\\nConditional: Must be set to true when the Digital Payment Application (DPA) processes in the United States (US)\\\"'\\n\"\n    },\n    \"supportedCheckoutTypes\": {\n      \"type\": \"array\",\n      \"description\": \"List of checkout types to be supported by the DPA. These include CLICK_TO_PAY, GUEST_CHECKOUT_TOKENIZATION and CARD_ON_FILE_TOKENIZATION.\"\
  \n    },\n    \"acquirerData\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-unified-checkout-solutions-dpa-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Dpa
---
