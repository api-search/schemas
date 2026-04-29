---
description: SweepConfigurationNotificationData schema from Adyen API
layout: schema
name: SweepConfigurationNotificationData
properties_list:
- description: The unique identifier of the balance account for which the sweep was configured.
  name: accountId
  type: string
- description: The unique identifier of the balance platform.
  name: balancePlatform
  type: string
- description: Contains information about the sweep resource that triggered the event.
  name: sweep
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-sweep-configuration-notification-data-schema.json
slug: configuration-webhooks-sweep-configuration-notification-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-sweep-configuration-notification-data-schema.json\",\n  \"title\": \"SweepConfigurationNotificationData\",\n  \"description\": \"SweepConfigurationNotificationData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"description\": \"The unique identifier of the balance account for which the sweep was configured.\",\n      \"type\": \"string\"\n    },\n    \"balancePlatform\": {\n      \"description\": \"The unique identifier of the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"sweep\": {\n      \"description\": \"Contains information about the sweep resource that triggered the event.\",\n      \"$ref\": \"#/components/schemas/SweepConfigurationV2\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-sweep-configuration-notification-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SweepConfigurationNotificationData
---
