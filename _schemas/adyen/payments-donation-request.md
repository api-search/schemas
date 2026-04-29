---
description: DonationRequest schema from Adyen API
layout: schema
name: DonationRequest
properties_list:
- description: The Adyen account name of the charity.
  name: donationAccount
  type: string
- description: The merchant account that is used to process the payment.
  name: merchantAccount
  type: string
- description: The amount to be donated.The `currency` must match the currency used in authorisation, the `value` must be smaller than or equal to the authorised amount.
  name: modificationAmount
  type: object
- description: 'The original pspReference of the payment to modify. This reference is returned in: * authorisation response * authorisation notification'
  name: originalReference
  type: string
- description: Defines how to book chargebacks when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#chargebacks-and-disputes).
  name: platformChargebackLogic
  type: object
- description: 'Your reference for the payment modification. This reference is visible in Customer Area and in reports. Maximum length: 80 characters.'
  name: reference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-donation-request-schema.json
slug: payments-donation-request
source_filename: payments-donation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-donation-request-schema.json\",\n  \"title\": \"DonationRequest\",\n  \"description\": \"DonationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"donationAccount\": {\n      \"description\": \"The Adyen account name of the charity.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account that is used to process the payment.\",\n      \"type\": \"string\"\n    },\n    \"modificationAmount\": {\n      \"description\": \"The amount to be donated.The `currency` must match the currency used in authorisation, the `value` must be smaller than or equal to the authorised amount.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"originalReference\": {\n      \"description\": \"The original pspReference of\
  \ the payment to modify.\\nThis reference is returned in:\\n* authorisation response\\n* authorisation notification\\n\\n\",\n      \"type\": \"string\"\n    },\n    \"platformChargebackLogic\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Defines how to book chargebacks when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#chargebacks-and-disputes).\",\n      \"$ref\": \"#/components/schemas/PlatformChargebackLogic\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the payment modification. This reference is visible in Customer Area and in reports.\\nMaximum length: 80 characters.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"donationAccount\",\n    \"modificationAmount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-donation-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DonationRequest
---
