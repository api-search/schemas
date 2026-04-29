---
description: AuthenticationNotificationRequest schema from Adyen API
layout: schema
name: AuthenticationNotificationRequest
properties_list:
- description: Contains event details.
  name: data
  type: object
- description: 'The environment from which the webhook originated. Possible values: **test**, **live**.'
  name: environment
  type: string
- description: Type of notification.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/authentication-webhooks-authentication-notification-request-schema.json
slug: authentication-webhooks-authentication-notification-request
source_filename: authentication-webhooks-authentication-notification-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/authentication-webhooks-authentication-notification-request-schema.json\",\n  \"title\": \"AuthenticationNotificationRequest\",\n  \"description\": \"AuthenticationNotificationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"Contains event details.\",\n      \"$ref\": \"#/components/schemas/AuthenticationNotificationData\"\n    },\n    \"environment\": {\n      \"description\": \"The environment from which the webhook originated.\\n\\nPossible values: **test**, **live**.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type of notification.\",\n      \"enum\": [\n        \"balancePlatform.authentication.created\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"environment\",\n  \
  \  \"type\",\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/authentication-webhooks-authentication-notification-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AuthenticationNotificationRequest
---
