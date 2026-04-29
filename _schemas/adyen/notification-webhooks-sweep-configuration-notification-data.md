---
description: SweepConfigurationNotificationData schema from Adyen API
layout: schema
name: SweepConfigurationNotificationData
properties_list:
- description: The unique identifier of the balance account for which the sweep was configured.
  name: accountId
  type: string
- description: Unique identifier of the balance platform.
  name: balancePlatform
  type: string
- description: Contains information about the sweep resource that triggered the event.
  name: sweep
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-sweep-configuration-notification-data-schema.json
slug: notification-webhooks-sweep-configuration-notification-data
source_filename: notification-webhooks-sweep-configuration-notification-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-sweep-configuration-notification-data-schema.json\",\n  \"title\": \"SweepConfigurationNotificationData\",\n  \"description\": \"SweepConfigurationNotificationData schema from Adyen API\",\n  \"properties\": {\n    \"accountId\": {\n      \"description\": \"The unique identifier of the balance account for which the sweep was configured.\",\n      \"type\": \"string\"\n    },\n    \"balancePlatform\": {\n      \"description\": \"Unique identifier of the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"sweep\": {\n      \"description\": \"Contains information about the sweep resource that triggered the event.\",\n      \"$ref\": \"#/components/schemas/SweepConfigurationV2\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-sweep-configuration-notification-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SweepConfigurationNotificationData
---
