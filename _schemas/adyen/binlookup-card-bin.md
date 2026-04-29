---
description: CardBin schema from Adyen API
layout: schema
name: CardBin
properties_list:
- description: The first 6 digit of the card number. Enable this field via merchant account settings.
  name: bin
  type: string
- description: If true, it indicates a commercial card. Enable this field via merchant account settings.
  name: commercial
  type: boolean
- description: 'The card funding source. Valid values are: * CHARGE * CREDIT * DEBIT * DEFERRED_DEBIT * PREPAID * PREPAID_RELOADABLE * PREPAID_NONRELOADABLE > Enable this field via merchant account settings.'
  name: fundingSource
  type: string
- description: 'Indicates availability of funds. Visa: * "I" (fast funds are supported) * "N" (otherwise) Mastercard: * "I" (product type is Prepaid or Debit, or issuing country is in CEE/HGEM list) * "N" (otherwise)'
  name: fundsAvailability
  type: string
- description: The first 8 digit of the card number. Enable this field via merchant account settings.
  name: issuerBin
  type: string
- description: The issuing bank of the card.
  name: issuingBank
  type: string
- description: The country where the card was issued from.
  name: issuingCountry
  type: string
- description: The currency of the card.
  name: issuingCurrency
  type: string
- description: The payment method associated with the card (e.g. visa, mc, or amex).
  name: paymentMethod
  type: string
- description: 'Indicates whether a payout is eligible or not for this card. Visa: * "Y" * "N" Mastercard: * "Y" (domestic and cross-border) * "D" (only domestic) * "N" (no MoneySend) * "U" (unknown) > Returned when '
  name: payoutEligible
  type: string
- description: The last four digits of the card number.
  name: summary
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/binlookup-card-bin-schema.json
slug: binlookup-card-bin
source_filename: binlookup-card-bin-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-card-bin-schema.json\",\n  \"title\": \"CardBin\",\n  \"description\": \"CardBin schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bin\": {\n      \"description\": \"The first 6 digit of the card number. Enable this field via merchant account settings.\",\n      \"type\": \"string\"\n    },\n    \"commercial\": {\n      \"description\": \"If true, it indicates a commercial card. Enable this field via merchant account settings.\",\n      \"type\": \"boolean\"\n    },\n    \"fundingSource\": {\n      \"description\": \"The card funding source. Valid values are:\\n* CHARGE\\n* CREDIT\\n* DEBIT\\n* DEFERRED_DEBIT\\n* PREPAID\\n* PREPAID_RELOADABLE\\n* PREPAID_NONRELOADABLE\\n> Enable this field via merchant account settings.\",\n      \"type\": \"string\"\n    },\n    \"fundsAvailability\"\
  : {\n      \"description\": \"Indicates availability of funds.\\n\\nVisa:\\n* \\\"I\\\" (fast funds are supported)\\n* \\\"N\\\" (otherwise)\\n\\nMastercard:\\n* \\\"I\\\" (product type is Prepaid or Debit, or issuing country is in CEE/HGEM list)\\n* \\\"N\\\" (otherwise)\\n> Returned when you verify a card BIN or estimate costs, and only if `payoutEligible` is different from \\\"N\\\" or \\\"U\\\".\",\n      \"type\": \"string\"\n    },\n    \"issuerBin\": {\n      \"x-addedInVersion\": \"54\",\n      \"description\": \"The first 8 digit of the card number. Enable this field via merchant account settings.\",\n      \"type\": \"string\"\n    },\n    \"issuingBank\": {\n      \"description\": \"The issuing bank of the card.\",\n      \"type\": \"string\"\n    },\n    \"issuingCountry\": {\n      \"description\": \"The country where the card was issued from.\",\n      \"type\": \"string\"\n    },\n    \"issuingCurrency\": {\n      \"description\": \"The currency of the card.\",\n      \"\
  type\": \"string\"\n    },\n    \"paymentMethod\": {\n      \"description\": \"The payment method associated with the card (e.g. visa, mc, or amex).\",\n      \"type\": \"string\"\n    },\n    \"payoutEligible\": {\n      \"description\": \"Indicates whether a payout is eligible or not for this card.\\n\\nVisa:\\n* \\\"Y\\\"\\n* \\\"N\\\"\\n\\nMastercard:\\n* \\\"Y\\\" (domestic and cross-border)\\n* \\\"D\\\" (only domestic)\\n* \\\"N\\\" (no MoneySend)\\n* \\\"U\\\" (unknown)\\n> Returned when you verify a card BIN or estimate costs, and only if `payoutEligible` is different from \\\"N\\\" or \\\"U\\\".\",\n      \"type\": \"string\"\n    },\n    \"summary\": {\n      \"description\": \"The last four digits of the card number.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-card-bin-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardBin
---
