---
description: ListStoredPaymentMethodsResponse schema from Adyen API
layout: schema
name: ListStoredPaymentMethodsResponse
properties_list:
- description: Your merchant account.
  name: merchantAccount
  type: string
- description: 'Your reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters. > Your reference must not include personally identifiable information (PII), for exam'
  name: shopperReference
  type: string
- description: List of all stored payment methods.
  name: storedPaymentMethods
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-list-stored-payment-methods-response-schema.json
slug: checkout-list-stored-payment-methods-response
source_filename: checkout-list-stored-payment-methods-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-list-stored-payment-methods-response-schema.json\",\n  \"title\": \"ListStoredPaymentMethodsResponse\",\n  \"description\": \"ListStoredPaymentMethodsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantAccount\": {\n      \"description\": \"Your merchant account.\",\n      \"type\": \"string\"\n    },\n    \"shopperReference\": {\n      \"description\": \"Your reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters.\\n> Your reference must not include personally identifiable information (PII), for example name or email address.\",\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethods\": {\n      \"description\": \"List of all stored payment methods.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StoredPaymentMethodResource\"\
  \n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-list-stored-payment-methods-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ListStoredPaymentMethodsResponse
---
