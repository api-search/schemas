---
description: A subscription offer represents special pricing for a subscription, such as a free trial or introductory price.
layout: schema
name: SubscriptionOffer
properties_list:
- description: The package name of the parent app.
  name: packageName
  type: string
- description: The product ID of the parent subscription.
  name: productId
  type: string
- description: The base plan ID the offer is associated with.
  name: basePlanId
  type: string
- description: The unique identifier for this offer.
  name: offerId
  type: string
- description: The current state of the offer.
  name: state
  type: string
- description: The pricing phases for this offer. Each phase defines a pricing period with its own duration and price.
  name: phases
  type: array
- description: Targeting rules for the offer.
  name: targeting
  type: object
- description: Regional configuration for this offer.
  name: regionalConfigs
  type: array
- description: Custom tags for this offer.
  name: offerTags
  type: array
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-subscription-offer-schema.json
slug: google-play-developer-subscription-offer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubscriptionOffer\",\n  \"type\": \"object\",\n  \"description\": \"A subscription offer represents special pricing for a subscription, such as a free trial or introductory price.\",\n  \"properties\": {\n    \"packageName\": {\n      \"type\": \"string\",\n      \"description\": \"The package name of the parent app.\"\n    },\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"The product ID of the parent subscription.\"\n    },\n    \"basePlanId\": {\n      \"type\": \"string\",\n      \"description\": \"The base plan ID the offer is associated with.\"\n    },\n    \"offerId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for this offer.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the offer.\"\n    },\n    \"phases\": {\n      \"type\": \"array\",\n      \"description\": \"\
  The pricing phases for this offer. Each phase defines a pricing period with its own duration and price.\"\n    },\n    \"targeting\": {\n      \"type\": \"object\",\n      \"description\": \"Targeting rules for the offer.\"\n    },\n    \"regionalConfigs\": {\n      \"type\": \"array\",\n      \"description\": \"Regional configuration for this offer.\"\n    },\n    \"offerTags\": {\n      \"type\": \"array\",\n      \"description\": \"Custom tags for this offer.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-subscription-offer-schema.json
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
title: SubscriptionOffer
---
