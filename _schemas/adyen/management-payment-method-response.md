---
description: PaymentMethodResponse schema from Adyen API
layout: schema
name: PaymentMethodResponse
properties_list:
- description: Pagination references.
  name: _links
  type: object
- description: The list of supported payment methods and their details.
  name: data
  type: array
- description: Total number of items.
  name: itemsTotal
  type: integer
- description: Total number of pages.
  name: pagesTotal
  type: integer
- description: Payment method types with errors.
  name: typesWithErrors
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-payment-method-response-schema.json
slug: management-payment-method-response
source_filename: management-payment-method-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-payment-method-response-schema.json\",\n  \"title\": \"PaymentMethodResponse\",\n  \"description\": \"PaymentMethodResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_links\": {\n      \"description\": \"Pagination references.\",\n      \"$ref\": \"#/components/schemas/PaginationLinks\"\n    },\n    \"data\": {\n      \"description\": \"The list of supported payment methods and their details.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PaymentMethod\"\n      },\n      \"type\": \"array\"\n    },\n    \"itemsTotal\": {\n      \"description\": \"Total number of items.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"pagesTotal\": {\n      \"description\": \"Total number of pages.\",\n      \"format\": \"int32\",\n     \
  \ \"type\": \"integer\"\n    },\n    \"typesWithErrors\": {\n      \"description\": \"Payment method types with errors.\",\n      \"items\": {\n        \"enum\": [\n          \"afterpaytouch\",\n          \"alipay\",\n          \"alipay_hk\",\n          \"amex\",\n          \"applepay\",\n          \"bcmc\",\n          \"blik\",\n          \"cartebancaire\",\n          \"clearpay\",\n          \"cup\",\n          \"diners\",\n          \"directdebit_GB\",\n          \"discover\",\n          \"ebanking_FI\",\n          \"eftpos_australia\",\n          \"elo\",\n          \"elocredit\",\n          \"elodebit\",\n          \"girocard\",\n          \"googlepay\",\n          \"hiper\",\n          \"hipercard\",\n          \"ideal\",\n          \"interac_card\",\n          \"jcb\",\n          \"klarna\",\n          \"klarna_account\",\n          \"klarna_paynow\",\n          \"maestro\",\n          \"mbway\",\n          \"mc\",\n          \"mcdebit\",\n          \"mealVoucher_FR\",\n       \
  \   \"mobilepay\",\n          \"multibanco\",\n          \"onlineBanking_PL\",\n          \"paybybank\",\n          \"paypal\",\n          \"payshop\",\n          \"swish\",\n          \"trustly\",\n          \"twint\",\n          \"twint_pos\",\n          \"vipps\",\n          \"visa\",\n          \"visadebit\",\n          \"vpay\",\n          \"wechatpay\",\n          \"wechatpay_pos\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"itemsTotal\",\n    \"pagesTotal\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-payment-method-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentMethodResponse
---
