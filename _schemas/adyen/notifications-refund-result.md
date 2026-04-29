---
description: RefundResult schema from Adyen API
layout: schema
name: RefundResult
properties_list:
- description: The transaction that has been refunded.
  name: originalTransaction
  type: object
- description: The reference of the refund.
  name: pspReference
  type: string
- description: The response indicating if the refund has been received for processing.
  name: response
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-refund-result-schema.json
slug: notifications-refund-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-refund-result-schema.json\",\n  \"title\": \"RefundResult\",\n  \"description\": \"RefundResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"originalTransaction\": {\n      \"description\": \"The transaction that has been refunded.\",\n      \"$ref\": \"#/components/schemas/Transaction\"\n    },\n    \"pspReference\": {\n      \"description\": \"The reference of the refund.\",\n      \"type\": \"string\"\n    },\n    \"response\": {\n      \"description\": \"The response indicating if the refund has been received for processing.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-refund-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RefundResult
---
