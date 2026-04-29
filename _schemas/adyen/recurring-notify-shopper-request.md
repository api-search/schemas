---
description: NotifyShopperRequest schema from Adyen API
layout: schema
name: NotifyShopperRequest
properties_list:
- description: The amount of the upcoming payment.
  name: amount
  type: object
- description: Date on which the subscription amount will be debited from the shopper. In YYYY-MM-DD format
  name: billingDate
  type: string
- description: Sequence of the debit. Depends on Frequency and Billing Attempts Rule.
  name: billingSequenceNumber
  type: string
- description: Reference of Pre-debit notification that is displayed to the shopper. Optional field. Maps to reference if missing
  name: displayedReference
  type: string
- description: The merchant account identifier with which you want to process the transaction.
  name: merchantAccount
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: recurringDetailReference
  type: string
- description: Pre-debit notification reference sent by the merchant. This is a mandatory field
  name: reference
  type: string
- description: The ID that uniquely identifies the shopper. This `shopperReference` must be the same as the `shopperReference` used in the initial payment.
  name: shopperReference
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: storedPaymentMethodId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-notify-shopper-request-schema.json
slug: recurring-notify-shopper-request
source_filename: recurring-notify-shopper-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-notify-shopper-request-schema.json\",\n  \"title\": \"NotifyShopperRequest\",\n  \"description\": \"NotifyShopperRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The amount of the upcoming payment.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"billingDate\": {\n      \"description\": \"Date on which the subscription amount will be debited from the shopper. In YYYY-MM-DD format\",\n      \"type\": \"string\"\n    },\n    \"billingSequenceNumber\": {\n      \"description\": \"Sequence of the debit. Depends on Frequency and Billing Attempts Rule.\",\n      \"type\": \"string\"\n    },\n    \"displayedReference\": {\n      \"description\": \"Reference of Pre-debit notification that is displayed to the shopper. Optional\
  \ field. Maps to reference if missing\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier with which you want to process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Pre-debit notification reference sent by the merchant. This is a mandatory field\",\n      \"type\": \"string\"\n    },\n    \"shopperReference\": {\n      \"description\": \"The ID that uniquely identifies the shopper.\\n\\nThis `shopperReference` must be the same as the `shopperReference` used in the initial payment.\",\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethodId\": {\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\"\
  ,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"shopperReference\",\n    \"amount\",\n    \"reference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-notify-shopper-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: NotifyShopperRequest
---
