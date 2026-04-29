---
description: MerchantDetails schema from Adyen API
layout: schema
name: MerchantDetails
properties_list:
- description: 2-letter ISO 3166 country code of the card acceptor location. > This parameter is required for the merchants who don't use Adyen as the payment authorisation gateway.
  name: countryCode
  type: string
- description: If true, indicates that the merchant is enrolled in 3D Secure for the card network.
  name: enrolledIn3DSecure
  type: boolean
- description: The merchant category code (MCC) is a four-digit number which relates to a particular market segment. This code reflects the predominant activity that is conducted by the merchant. The list of MCCs ca
  name: mcc
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/binlookup-merchant-details-schema.json
slug: binlookup-merchant-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-merchant-details-schema.json\",\n  \"title\": \"MerchantDetails\",\n  \"description\": \"MerchantDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"countryCode\": {\n      \"description\": \"2-letter ISO 3166 country code of the card acceptor location.\\n> This parameter is required for the merchants who don't use Adyen as the payment authorisation gateway.\",\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"enrolledIn3DSecure\": {\n      \"description\": \"If true, indicates that the merchant is enrolled in 3D Secure for the card network.\",\n      \"type\": \"boolean\"\n    },\n    \"mcc\": {\n      \"description\": \"The merchant category code (MCC) is a four-digit number which relates to a particular market segment. This\
  \ code reflects the predominant activity that is conducted by the merchant.\\n\\nThe list of MCCs can be found [here](https://en.wikipedia.org/wiki/Merchant_category_code).\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-merchant-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MerchantDetails
---
