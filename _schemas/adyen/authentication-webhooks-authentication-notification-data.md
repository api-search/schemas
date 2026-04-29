---
description: AuthenticationNotificationData schema from Adyen API
layout: schema
name: AuthenticationNotificationData
properties_list:
- description: Information about the authentication.
  name: authentication
  type: object
- description: The unique identifier of the balance platform.
  name: balancePlatform
  type: string
- description: Unique identifier of the authentication.
  name: id
  type: string
- description: Unique identifier of the payment instrument that was used for the authentication.
  name: paymentInstrumentId
  type: string
- description: Information about the purchase.
  name: purchase
  type: object
- description: 'Outcome of the authentication. Allowed values: * authenticated * rejected * error'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/authentication-webhooks-authentication-notification-data-schema.json
slug: authentication-webhooks-authentication-notification-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/authentication-webhooks-authentication-notification-data-schema.json\",\n  \"title\": \"AuthenticationNotificationData\",\n  \"description\": \"AuthenticationNotificationData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authentication\": {\n      \"description\": \"Information about the authentication.\",\n      \"$ref\": \"#/components/schemas/AuthenticationInfo\"\n    },\n    \"balancePlatform\": {\n      \"description\": \"The unique identifier of the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"Unique identifier of the authentication.\",\n      \"type\": \"string\"\n    },\n    \"paymentInstrumentId\": {\n      \"description\": \"Unique identifier of the payment instrument that was used for the authentication.\",\n      \"\
  type\": \"string\"\n    },\n    \"purchase\": {\n      \"description\": \"Information about the purchase.\",\n      \"$ref\": \"#/components/schemas/PurchaseInfo\"\n    },\n    \"status\": {\n      \"description\": \"Outcome of the authentication.\\nAllowed values:\\n* authenticated\\n* rejected\\n* error\",\n      \"enum\": [\n        \"authenticated\",\n        \"rejected\",\n        \"error\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"paymentInstrumentId\",\n    \"status\",\n    \"authentication\",\n    \"purchase\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/authentication-webhooks-authentication-notification-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AuthenticationNotificationData
---
