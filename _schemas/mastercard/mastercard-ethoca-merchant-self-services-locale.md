---
description: Merchant Locale details
layout: schema
name: Locale
properties_list:
- description: The locale where the merchant anticipates their business to be located; often referred to as the Accept-Language in HTTP headers.
  name: code
  type: string
- description: Description of the primary merchant tied to the transaction and responsible for providing the products or services (description of the business, what they do, markets, etc.). Used to help cardholder u
  name: merchantDescription
  type: string
- description: This indicates whether or not this locale will be used as the default locale for displaying information to the customer.
  name: defaultLocale
  type: boolean
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-locale-schema.json
slug: mastercard-ethoca-merchant-self-services-locale
source_filename: mastercard-ethoca-merchant-self-services-locale-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Locale\",\n  \"type\": \"object\",\n  \"description\": \"Merchant Locale details\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The locale where the merchant anticipates their business to be located; often referred to as the Accept-Language in HTTP headers.\"\n    },\n    \"merchantDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the primary merchant tied to the transaction and responsible for providing the products or services (description of the business, what they do, markets, etc.). Used to help cardholder understand business responsible for the charge.\"\n    },\n    \"defaultLocale\": {\n      \"type\": \"boolean\",\n      \"description\": \"This indicates whether or not this locale will be used as the default locale for displaying information to the customer.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-locale-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Locale
---
