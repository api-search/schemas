---
description: ResponseAdditionalDataCard schema from Adyen API
layout: schema
name: ResponseAdditionalDataCard
properties_list:
- description: 'The first six digits of the card number. This is the [Bank Identification Number (BIN)](https://docs.adyen.com/get-started-with-adyen/payment-glossary#bank-identification-number-bin) for card numbers '
  name: cardBin
  type: string
- description: The cardholder name passed in the payment request.
  name: cardHolderName
  type: string
- description: The bank or the financial institution granting lines of credit through card association branded payment cards. This information can be included when available.
  name: cardIssuingBank
  type: string
- description: 'The country where the card was issued. Example: US'
  name: cardIssuingCountry
  type: string
- description: 'The currency in which the card is issued, if this information is available. Provided as the currency code or currency number from the ISO-4217 standard. Example: USD'
  name: cardIssuingCurrency
  type: string
- description: 'The card payment method used for the transaction. Example: amex'
  name: cardPaymentMethod
  type: string
- description: The last four digits of a card number. > Returned only in case of a card payment.
  name: cardSummary
  type: string
- description: The first eight digits of the card number. Only returned if the card number is 16 digits or more. This is the [Bank Identification Number (BIN)](https://docs.adyen.com/get-started-with-adyen/payment-g
  name: issuerBin
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payouts-response-additional-data-card-schema.json
slug: payouts-response-additional-data-card
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-response-additional-data-card-schema.json\",\n  \"title\": \"ResponseAdditionalDataCard\",\n  \"description\": \"ResponseAdditionalDataCard schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardBin\": {\n      \"description\": \"The first six digits of the card number.\\n\\nThis is the [Bank Identification Number (BIN)](https://docs.adyen.com/get-started-with-adyen/payment-glossary#bank-identification-number-bin) for card numbers with a six-digit BIN.\\n\\nExample: 521234\",\n      \"type\": \"string\"\n    },\n    \"cardHolderName\": {\n      \"description\": \"The cardholder name passed in the payment request.\",\n      \"type\": \"string\"\n    },\n    \"cardIssuingBank\": {\n      \"description\": \"The bank or the financial institution granting lines of credit through card\
  \ association branded payment cards. This information can be included when available.\",\n      \"type\": \"string\"\n    },\n    \"cardIssuingCountry\": {\n      \"description\": \"The country where the card was issued.\\n\\nExample: US\",\n      \"type\": \"string\"\n    },\n    \"cardIssuingCurrency\": {\n      \"description\": \"The currency in which the card is issued, if this information is available. Provided as the currency code or currency number from the ISO-4217 standard. \\n\\nExample: USD\",\n      \"type\": \"string\"\n    },\n    \"cardPaymentMethod\": {\n      \"description\": \"The card payment method used for the transaction.\\n\\nExample: amex\",\n      \"type\": \"string\"\n    },\n    \"cardSummary\": {\n      \"description\": \"The last four digits of a card number.\\n\\n> Returned only in case of a card payment.\",\n      \"type\": \"string\"\n    },\n    \"issuerBin\": {\n      \"description\": \"The first eight digits of the card number. Only returned if the card\
  \ number is 16 digits or more.\\n\\nThis is the [Bank Identification Number (BIN)](https://docs.adyen.com/get-started-with-adyen/payment-glossary#bank-identification-number-bin) for card numbers with an eight-digit BIN.\\n\\nExample: 52123423\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-response-additional-data-card-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ResponseAdditionalDataCard
---
