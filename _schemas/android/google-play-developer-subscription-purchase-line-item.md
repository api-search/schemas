---
description: An individual line item within a v2 subscription purchase. Each line item represents a base plan or offer.
layout: schema
name: SubscriptionPurchaseLineItem
properties_list:
- description: The product ID of the subscription.
  name: productId
  type: string
- description: Time at which the subscription line item will expire.
  name: expiryTime
  type: string
- description: Details for auto-renewing plans.
  name: autoRenewingPlan
  type: object
- description: Details for prepaid plans.
  name: prepaidPlan
  type: object
- description: Details of the offer applied to this line item.
  name: offerDetails
  type: object
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-subscription-purchase-line-item-schema.json
slug: google-play-developer-subscription-purchase-line-item
source_filename: google-play-developer-subscription-purchase-line-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubscriptionPurchaseLineItem\",\n  \"type\": \"object\",\n  \"description\": \"An individual line item within a v2 subscription purchase. Each line item represents a base plan or offer.\",\n  \"properties\": {\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"The product ID of the subscription.\"\n    },\n    \"expiryTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time at which the subscription line item will expire.\"\n    },\n    \"autoRenewingPlan\": {\n      \"type\": \"object\",\n      \"description\": \"Details for auto-renewing plans.\"\n    },\n    \"prepaidPlan\": {\n      \"type\": \"object\",\n      \"description\": \"Details for prepaid plans.\"\n    },\n    \"offerDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Details of the offer applied to this line item.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-subscription-purchase-line-item-schema.json
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
title: SubscriptionPurchaseLineItem
---
