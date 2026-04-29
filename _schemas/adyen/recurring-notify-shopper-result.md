---
description: NotifyShopperResult schema from Adyen API
layout: schema
name: NotifyShopperResult
properties_list:
- description: Reference of Pre-debit notification that is displayed to the shopper
  name: displayedReference
  type: string
- description: A simple description of the `resultCode`.
  name: message
  type: string
- description: The unique reference that is associated with the request.
  name: pspReference
  type: string
- description: Reference of Pre-debit notification sent in my the merchant
  name: reference
  type: string
- description: The code indicating the status of notification.
  name: resultCode
  type: string
- description: The unique reference for the request sent downstream.
  name: shopperNotificationReference
  type: string
- description: This is the recurringDetailReference returned in the response when token was created
  name: storedPaymentMethodId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-notify-shopper-result-schema.json
slug: recurring-notify-shopper-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-notify-shopper-result-schema.json\",\n  \"title\": \"NotifyShopperResult\",\n  \"description\": \"NotifyShopperResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayedReference\": {\n      \"description\": \"Reference of Pre-debit notification that is displayed to the shopper\",\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"description\": \"A simple description of the `resultCode`.\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"The unique reference that is associated with the request.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Reference of Pre-debit notification sent in my the merchant\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\"\
  : \"The code indicating the status of notification.\",\n      \"type\": \"string\"\n    },\n    \"shopperNotificationReference\": {\n      \"description\": \"The unique reference for the request sent downstream.\",\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethodId\": {\n      \"description\": \"This is the recurringDetailReference returned in the response when token was created\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-notify-shopper-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: NotifyShopperResult
---
