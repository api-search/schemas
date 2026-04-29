---
description: GetOnboardingUrlResponse schema from Adyen API
layout: schema
name: GetOnboardingUrlResponse
properties_list:
- description: Information about any invalid fields.
  name: invalidFields
  type: array
- description: The reference of a request. Can be used to uniquely identify the request.
  name: pspReference
  type: string
- description: The URL to the Hosted Onboarding Page where you should redirect your sub-merchant. This URL must be used within 30 seconds and can only be used once.
  name: redirectUrl
  type: string
- description: The result code.
  name: resultCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/hosted-onboarding-get-onboarding-url-response-schema.json
slug: hosted-onboarding-get-onboarding-url-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/hosted-onboarding-get-onboarding-url-response-schema.json\",\n  \"title\": \"GetOnboardingUrlResponse\",\n  \"description\": \"GetOnboardingUrlResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Information about any invalid fields.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"pspReference\": {\n      \"description\": \"The reference of a request. Can be used to uniquely identify the request.\",\n      \"type\": \"string\"\n    },\n    \"redirectUrl\": {\n      \"description\": \"The URL to the Hosted Onboarding Page where you should redirect your sub-merchant. This URL must be used within 30 seconds and can only\
  \ be used once.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/hosted-onboarding-get-onboarding-url-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetOnboardingUrlResponse
---
