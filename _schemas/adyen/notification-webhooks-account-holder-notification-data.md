---
description: AccountHolderNotificationData schema from Adyen API
layout: schema
name: AccountHolderNotificationData
properties_list:
- description: Contains information about the account holder resource that triggered the event.
  name: accountHolder
  type: object
- description: Unique identifier of the balance platform.
  name: balancePlatform
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-account-holder-notification-data-schema.json
slug: notification-webhooks-account-holder-notification-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-account-holder-notification-data-schema.json\",\n  \"title\": \"AccountHolderNotificationData\",\n  \"description\": \"AccountHolderNotificationData schema from Adyen API\",\n  \"properties\": {\n    \"accountHolder\": {\n      \"description\": \"Contains information about the account holder resource that triggered the event.\",\n      \"$ref\": \"#/components/schemas/AccountHolder\"\n    },\n    \"balancePlatform\": {\n      \"description\": \"Unique identifier of the balance platform.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-account-holder-notification-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderNotificationData
---
