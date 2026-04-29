---
description: PaginatedPaymentInstrumentsResponse schema from Adyen API
layout: schema
name: PaginatedPaymentInstrumentsResponse
properties_list:
- description: Indicates whether there are more items on the next page.
  name: hasNext
  type: boolean
- description: Indicates whether there are more items on the previous page.
  name: hasPrevious
  type: boolean
- description: List of payment instruments associated with the balance account.
  name: paymentInstruments
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-paginated-payment-instruments-response-schema.json
slug: configuration-paginated-payment-instruments-response
source_filename: configuration-paginated-payment-instruments-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-paginated-payment-instruments-response-schema.json\",\n  \"title\": \"PaginatedPaymentInstrumentsResponse\",\n  \"description\": \"PaginatedPaymentInstrumentsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hasNext\": {\n      \"description\": \"Indicates whether there are more items on the next page.\",\n      \"type\": \"boolean\"\n    },\n    \"hasPrevious\": {\n      \"description\": \"Indicates whether there are more items on the previous page.\",\n      \"type\": \"boolean\"\n    },\n    \"paymentInstruments\": {\n      \"description\": \"List of payment instruments associated with the balance account.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PaymentInstrument\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n\
  \    \"paymentInstruments\",\n    \"hasPrevious\",\n    \"hasNext\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-paginated-payment-instruments-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaginatedPaymentInstrumentsResponse
---
