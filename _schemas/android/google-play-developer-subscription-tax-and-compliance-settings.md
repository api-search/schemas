---
description: Tax and compliance settings for a subscription.
layout: schema
name: SubscriptionTaxAndComplianceSettings
properties_list:
- description: Digital content or service classification for EEA withdrawal right.
  name: eeaWithdrawalRightType
  type: string
- description: Tax rate information keyed by region code.
  name: taxRateInfoByRegionCode
  type: object
- description: Whether the subscription represents a tokenized digital asset.
  name: isTokenizedDigitalAsset
  type: boolean
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-subscription-tax-and-compliance-settings-schema.json
slug: google-play-developer-subscription-tax-and-compliance-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubscriptionTaxAndComplianceSettings\",\n  \"type\": \"object\",\n  \"description\": \"Tax and compliance settings for a subscription.\",\n  \"properties\": {\n    \"eeaWithdrawalRightType\": {\n      \"type\": \"string\",\n      \"description\": \"Digital content or service classification for EEA withdrawal right.\"\n    },\n    \"taxRateInfoByRegionCode\": {\n      \"type\": \"object\",\n      \"description\": \"Tax rate information keyed by region code.\"\n    },\n    \"isTokenizedDigitalAsset\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the subscription represents a tokenized digital asset.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-subscription-tax-and-compliance-settings-schema.json
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
title: SubscriptionTaxAndComplianceSettings
---
