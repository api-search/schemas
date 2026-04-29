---
description: A purchase that has been voided (cancelled, refunded, or charged back).
layout: schema
name: VoidedPurchase
properties_list:
- description: Resource type identifier.
  name: kind
  type: string
- description: The token which uniquely identifies the purchase.
  name: purchaseToken
  type: string
- description: Time at which the purchase was made (milliseconds since Epoch).
  name: purchaseTimeMillis
  type: string
- description: Time at which the purchase was voided (milliseconds since Epoch).
  name: voidedTimeMillis
  type: string
- description: The order ID associated with the voided purchase.
  name: orderId
  type: string
- description: The source of the voiding. 0 = User, 1 = Developer, 2 = Google.
  name: voidedSource
  type: integer
- description: The reason for voiding. 0 = Other, 1 = Remorse, 2 = Not received, 3 = Defective, 4 = Accidental purchase, 5 = Fraud, 6 = Friendly fraud, 7 = Chargeback.
  name: voidedReason
  type: integer
- description: The voided quantity as related to multi-quantity purchases.
  name: voidedQuantity
  type: integer
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-voided-purchase-schema.json
slug: google-play-developer-voided-purchase
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VoidedPurchase\",\n  \"type\": \"object\",\n  \"description\": \"A purchase that has been voided (cancelled, refunded, or charged back).\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type identifier.\"\n    },\n    \"purchaseToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token which uniquely identifies the purchase.\"\n    },\n    \"purchaseTimeMillis\": {\n      \"type\": \"string\",\n      \"description\": \"Time at which the purchase was made (milliseconds since Epoch).\"\n    },\n    \"voidedTimeMillis\": {\n      \"type\": \"string\",\n      \"description\": \"Time at which the purchase was voided (milliseconds since Epoch).\"\n    },\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"The order ID associated with the voided purchase.\"\n    },\n    \"voidedSource\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"The source of the voiding. 0 = User, 1 = Developer, 2 = Google.\"\n    },\n    \"voidedReason\": {\n      \"type\": \"integer\",\n      \"description\": \"The reason for voiding. 0 = Other, 1 = Remorse, 2 = Not received, 3 = Defective, 4 = Accidental purchase, 5 = Fraud, 6 = Friendly fraud, 7 = Chargeback.\"\n    },\n    \"voidedQuantity\": {\n      \"type\": \"integer\",\n      \"description\": \"The voided quantity as related to multi-quantity purchases.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-voided-purchase-schema.json
tags:
- AI
- Android
- Automotive
- Google
- Machine Learning
- Mobile Development
- SDK
- TV
- Wearables
title: VoidedPurchase
---
