---
description: TransferNotificationTransferTracking schema from Adyen API
layout: schema
name: TransferNotificationTransferTracking
properties_list:
- description: The tracking status of the transfer.
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounting-notifications-transfer-notification-transfer-tracking-schema.json
slug: accounting-notifications-transfer-notification-transfer-tracking
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-transfer-notification-transfer-tracking-schema.json\",\n  \"title\": \"TransferNotificationTransferTracking\",\n  \"description\": \"TransferNotificationTransferTracking schema from Adyen API\",\n  \"properties\": {\n    \"status\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The tracking status of the transfer.\",\n      \"enum\": [\n        \"credited\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-transfer-notification-transfer-tracking-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferNotificationTransferTracking
---
