---
description: Represents an in-app product purchase. Contains the purchase state, consumption status, and order information.
layout: schema
name: ProductPurchase
properties_list:
- description: Resource type identifier.
  name: kind
  type: string
- description: Time the product was purchased (milliseconds since Epoch).
  name: purchaseTimeMillis
  type: string
- description: The purchase state of the order. 0 = Purchased, 1 = Canceled, 2 = Pending.
  name: purchaseState
  type: integer
- description: The consumption state of the in-app product. 0 = Yet to be consumed, 1 = Consumed.
  name: consumptionState
  type: integer
- description: Developer-specified string for additional transaction information.
  name: developerPayload
  type: string
- description: The order ID associated with the purchase.
  name: orderId
  type: string
- description: The type of purchase. 0 = Test (sandbox), 1 = Promo, 2 = Rewarded.
  name: purchaseType
  type: integer
- description: The acknowledgement state of the in-app product. 0 = Yet to be acknowledged, 1 = Acknowledged.
  name: acknowledgementState
  type: integer
- description: The purchase token generated at the time of purchase.
  name: purchaseToken
  type: string
- description: The in-app product SKU.
  name: productId
  type: string
- description: The quantity associated with the purchase.
  name: quantity
  type: integer
- description: An obfuscated version of the ID uniquely associated with the user's account in your app.
  name: obfuscatedExternalAccountId
  type: string
- description: An obfuscated version of the ID uniquely associated with the user's profile in your app.
  name: obfuscatedExternalProfileId
  type: string
- description: ISO 3166-1 alpha-2 billing region code of the user.
  name: regionCode
  type: string
- description: The quantity eligible for refund.
  name: refundableQuantity
  type: integer
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-product-purchase-schema.json
slug: google-play-developer-product-purchase
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProductPurchase\",\n  \"type\": \"object\",\n  \"description\": \"Represents an in-app product purchase. Contains the purchase state, consumption status, and order information.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type identifier.\"\n    },\n    \"purchaseTimeMillis\": {\n      \"type\": \"string\",\n      \"description\": \"Time the product was purchased (milliseconds since Epoch).\"\n    },\n    \"purchaseState\": {\n      \"type\": \"integer\",\n      \"description\": \"The purchase state of the order. 0 = Purchased, 1 = Canceled, 2 = Pending.\"\n    },\n    \"consumptionState\": {\n      \"type\": \"integer\",\n      \"description\": \"The consumption state of the in-app product. 0 = Yet to be consumed, 1 = Consumed.\"\n    },\n    \"developerPayload\": {\n      \"type\": \"string\",\n      \"description\": \"Developer-specified\
  \ string for additional transaction information.\"\n    },\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"The order ID associated with the purchase.\"\n    },\n    \"purchaseType\": {\n      \"type\": \"integer\",\n      \"description\": \"The type of purchase. 0 = Test (sandbox), 1 = Promo, 2 = Rewarded.\"\n    },\n    \"acknowledgementState\": {\n      \"type\": \"integer\",\n      \"description\": \"The acknowledgement state of the in-app product. 0 = Yet to be acknowledged, 1 = Acknowledged.\"\n    },\n    \"purchaseToken\": {\n      \"type\": \"string\",\n      \"description\": \"The purchase token generated at the time of purchase.\"\n    },\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"The in-app product SKU.\"\n    },\n    \"quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"The quantity associated with the purchase.\"\n    },\n    \"obfuscatedExternalAccountId\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"An obfuscated version of the ID uniquely associated with the user's account in your app.\"\n    },\n    \"obfuscatedExternalProfileId\": {\n      \"type\": \"string\",\n      \"description\": \"An obfuscated version of the ID uniquely associated with the user's profile in your app.\"\n    },\n    \"regionCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 billing region code of the user.\"\n    },\n    \"refundableQuantity\": {\n      \"type\": \"integer\",\n      \"description\": \"The quantity eligible for refund.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-product-purchase-schema.json
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
title: ProductPurchase
---
